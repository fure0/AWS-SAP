# CloudFront 동적 컨텐츠 캐싱 정리

## 1. 기본 개념
CloudFront는 정적 컨텐츠뿐 아니라 **동적 컨텐츠의 응답(Response)도 캐시할 수 있다.**

동적 컨텐츠는 요청에 따라 결과가 달라지지만, **같은 요청이면 일정 시간 동안 동일한 결과가 반환되는 경우**가 많기 때문이다.

---

## 2. 캐시 동작 방식

CloudFront는 **요청(Request)을 기준으로 응답(Response)을 캐시한다.**

예시 요청

GET /api/product?id=100

Origin 응답

{
  "id": 100,
  "price": 1000
}

CloudFront는 다음을 캐시한다.

요청  
GET /api/product?id=100  

응답  
{
  "id": 100,
  "price": 1000
}

이후 동일한 요청이 오면 Origin 서버를 호출하지 않고 **캐시된 응답을 반환한다.**

---

## 3. TTL(Time To Live)

캐시는 **TTL 동안 유지된다.**

예시

TTL = 60초

동작 흐름

0초  
CloudFront → Origin 호출  
price = 1000  
→ 캐시 저장  

20초  
Origin DB 변경  
price = 2000  

30초 요청  
CloudFront → 캐시 응답  
price = 1000  

TTL이 끝나기 전까지는 **Origin 데이터가 변경되어도 캐시된 응답을 계속 사용한다.**

---

## 4. TTL 만료 후 동작

TTL이 끝나면 다음 요청에서 Origin을 다시 호출한다.

61초 요청

User → CloudFront → Origin  
→ price = 2000  
→ 캐시 갱신

---

## 5. 캐시 전략

### 1) TTL을 짧게 설정
예

TTL = 10초

장점  
- 데이터 최신성 유지

단점  
- Origin 서버 호출 증가

---

### 2) Cache Invalidation 사용

데이터가 변경될 때 CloudFront 캐시를 삭제한다.

예

/api/product/100

Invalidate 후 다음 요청

User → CloudFront → Origin 호출

---

## 핵심 정리

CloudFront 캐시는 **Origin의 현재 상태가 아니라 일정 시간 동안의 응답 스냅샷을 저장하는 것**이다.
