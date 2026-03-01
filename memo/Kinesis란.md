# Kinesis 란?

**Amazon Web Services(AWS)의 Kinesis**는
👉 **실시간(Real-time)으로 대량의 데이터를 수집·처리·분석하기 위한 스트리밍 데이터 플랫폼**이에요.

쉽게 말해,

> “계속 흘러들어오는 데이터를 지연 없이 받아서 바로 처리하는 파이프라인”

---

## Kinesis가 필요한 상황은?

다음처럼 **데이터가 끊임없이 발생**하는 경우에 사용합니다.

* 웹/모바일 **접속 로그**
* IoT 센서 데이터
* 결제·주문 이벤트
* 서버/애플리케이션 로그
* 실시간 모니터링, 알림, 대시보드

---

## Kinesis의 핵심 개념

* **Stream(스트림)**: 데이터가 흘러가는 통로
* **Record(레코드)**: 개별 데이터 단위
* **Shard(샤드)**: 처리량 단위 (확장/성능과 직결)
* **Producer / Consumer**

  * Producer: 데이터를 넣는 쪽
  * Consumer: 데이터를 읽어 처리하는 쪽

---

## Kinesis 서비스 종류 (중요)

Kinesis는 “패키지 이름”이고, 실제로는 여러 서비스가 있어요.

### 1️⃣ **Amazon Kinesis Data Streams**

* **가장 기본**
* 실시간 데이터 스트리밍 처리
* 소비자가 직접 데이터를 읽어 처리
* Lambda, EC2, ECS, Analytics와 연동

📌 예:

```
웹 서버 → Kinesis Data Streams → Lambda → DynamoDB
```

---

### 2️⃣ **Amazon Kinesis Data Firehose**

* **저장 목적**
* 스트리밍 데이터를 자동으로 목적지로 전달
* S3, Redshift, OpenSearch 등

📌 특징

* 서버 관리 거의 없음
* 실시간 처리보다는 **적재(Delivery)** 중심

---

### 3️⃣ **Amazon Kinesis Data Analytics**

* 스트리밍 데이터에 **SQL / Apache Flink** 적용
* 실시간 집계, 윈도우 분석

📌 예:

```
1분간 주문 수, 평균 응답시간 계산
```

---

### 4️⃣ **Amazon Kinesis Video Streams**

* 영상/음성 스트리밍 전용
* CCTV, 드론, 영상 분석

---

## Kinesis vs SQS / Kafka (간단 비교)

| 항목      | Kinesis      | SQS   | Kafka |
| ------- | ------------ | ----- | ----- |
| 실시간 스트림 | ✅            | ❌     | ✅     |
| 순서 보장   | ✅ (Shard 단위) | ❌     | ✅     |
| 재처리     | 가능           | 어려움   | 가능    |
| 운영 부담   | 낮음           | 매우 낮음 | 높음    |

---

## 언제 Kinesis를 쓰면 좋을까?

✅ **실시간 처리 필요**
✅ **로그·이벤트가 초당 수천~수만 건**
✅ **AWS 내 서비스와 연계**
❌ 단순 비동기 큐면 → SQS가 더 적합

---

## 한 줄 요약

> **Kinesis는 AWS에서 실시간 데이터 스트림을 처리하기 위한 핵심 서비스 묶음**이다.