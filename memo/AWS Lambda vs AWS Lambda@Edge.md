## 1️⃣ AWS Lambda vs AWS Lambda@Edge

### ✅ AWS Lambda

* 서버 없이 코드 실행하는 서비스
* 리전에 배포 (예: ap-northeast-1 도쿄)
* API, 배치, 이벤트 처리 등에 사용
* S3, DynamoDB, EventBridge 등과 연동

---

### ✅ AWS Lambda@Edge

* Lambda의 **특수한 형태**
* **CloudFront 엣지 로케이션에서 실행**
* CDN 요청/응답을 가로채서 처리 가능

반드시
👉 Amazon CloudFront 와 함께 사용해야 함

---

## 2️⃣ 가장 큰 차이

| 구분    | Lambda            | Lambda@Edge           |
| ----- | ----------------- | --------------------- |
| 실행 위치 | 특정 리전             | 전 세계 CloudFront 엣지    |
| 주요 목적 | 백엔드 로직            | CDN 요청/응답 조작          |
| 트리거   | API Gateway, S3 등 | CloudFront            |
| 배포 위치 | 아무 리전 가능          | 반드시 us-east-1에 생성     |
| 용도 예  | API 서버            | 리다이렉트, 헤더 조작, A/B 테스트 |

---

## 3️⃣ 언제 Lambda@Edge를 쓰나?

예를 들면:

* 국가별 리다이렉트
* 요청 헤더 수정
* 쿠키 기반 A/B 테스트
* 이미지 요청 URL 변경
* 보안 헤더 삽입

즉, **"CDN 레벨에서 처리하고 싶을 때"** 사용해.

---

## 4️⃣ 시험 관점 (SAA 기준)

네가 AWS SAA 이미 합격했으니까 정리해주면 👇

* 글로벌 엣지에서 실행 → **Lambda@Edge**
* API 처리 → **Lambda**
* 단순 헤더 조작 → Lambda@Edge
* 이미지 리사이징 → 상황에 따라 둘 다 가능

---

## 5️⃣ 핵심 한 줄 정리

> 🔹 Lambda@Edge는 Lambda의 한 종류다
> 🔹 일반 Lambda를 뜻하는 말은 아니다
> 🔹 CloudFront 전용 Lambda라고 보면 이해 쉬움
