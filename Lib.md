## 3.자격증명 & 페더레이션

  ### IAM (Identity and Access Management)
  > AWS 리소스에 대한 사용자, 그룹, 역할 및 권한을 중앙에서 관리하는 서비스

  ### IAM Access Anayzer
  > S3, IAM, KMS 등 리소스가 외부에 과도하게 공개되어 있는지 분석해 주는 보안 점검 도구

  ### STS (Security Token Service)
  > 사용자나 역할에게 짧은 시간 동안만 유효한 임시 보안 자격 증명을 발급하는 서비스

  ### (AWS) 디렉터리 서비스
  > 온프레미스 또는 클라우드 디렉터리(AD 등)와 연동해 중앙 사용자 인증을 제공하는 서비스

  ### (AWS) Organizations
  > 여러 AWS 계정을 조직 단위로 묶어 정책, 보안, 결제를 중앙에서 관리하는 서비스

  ### IAM Identity Center
  > 여러 AWS 계정과 SaaS 애플리케이션에 싱글사인온(SSO)을 제공하는 중앙 인증·권한 서비스

  ### (AWS) 컨트롤 타워
  > 모범 사례에 맞는 멀티 계정 환경(랜딩존)을 자동으로 구축하고 거버넌스를 적용하는 서비스

  ### (AWS) RAM (리소스 액세스 매니저)
  > 서브넷, 라이선스 등 리소스를 다른 계정과 안전하게 공유할 수 있게 해주는 서비스

## 4.보안

  ### CloudTrail
  > 계정 내에서 발생하는 API 호출과 콘솔 활동을 기록해 감사·보안 분석에 사용하는 서비스

  ### KMS (Key Management Service)
  > 데이터 암호화를 위한 키를 생성·저장·관리하는 관리형 키 관리 서비스

  ### 파라미터 스토어
  > 애플리케이션 설정값과 비밀값을 안전하게 저장하고 버전 관리하는 구성 저장소

  ### ACM (AWS Certificate Manager)
  > SSL/TLS 인증서를 자동으로 발급·배포·갱신해 주는 인증서 관리 서비스

  ### CloudHSM
  > 전용 HSM 하드웨어에서 암호 키를 관리하는 하드웨어 보안 모듈 서비스

  ### (AWS) Shield
  > DDoS 공격으로부터 애플리케이션을 보호하는 관리형 DDoS 방어 서비스

  ### (AWS) WAF
  > 웹 애플리케이션에 대한 SQL 인젝션, XSS 등을 차단하는 웹 방화벽 서비스

  ### Firewall Manager
  > 여러 계정·리전에 걸친 WAF, Shield, VPC 보안 정책을 중앙에서 일괄 관리하는 서비스

  ### (Amazon) Inspector
  > EC2, 컨테이너 이미지 등의 취약점과 보안 모범 사례 위반을 자동으로 스캔하는 서비스

  ### (AWS) Config
  > 리소스 구성 변경 이력을 추적하고 규정 준수 여부를 평가하는 설정 감시 서비스

  ### GuardDuty
  > 계정·네트워크·로그를 분석해 이상 징후와 잠재 위협을 탐지하는 지능형 위협 탐지 서비스

  ### EC2 Instance Connect
  > SSH 키를 직접 배포하지 않고도 안전하게 EC2 인스턴스에 접속할 수 있게 해주는 기능

  ### (AWS) Security Hub
  > 여러 보안 서비스의 결과를 모아 계정 전반의 보안 상태를 중앙 대시보드로 제공하는 서비스

  ### (Amazon) Detective
  > GuardDuty, CloudTrail 등의 로그를 분석해 보안 사건의 원인과 연관성을 시각적으로 조사하는 서비스

## 5.컴퓨팅&로드밸런싱

  ### ECR (Elastic Container Registry)
  > Docker 컨테이너 이미지를 저장·버전 관리하는 완전관리형 컨테이너 레지스트리

  ### EKS (Ekastic Kubernetes)
  > Kubernetes 클러스터의 컨트롤 플레인을 AWS가 대신 운영해 주는 관리형 K8s 서비스

  ### (AWS)-App-Runnber
  > 컨테이너나 소스 코드만 올리면 자동으로 스케일링되는 웹 애플리케이션 실행 서비스

  ### (AWS) Lambda
  > 서버를 직접 관리하지 않고 이벤트에 따라 코드를 실행하는 서버리스 컴퓨팅 서비스

  ### API Gateway
  > REST, HTTP, WebSocket API를 만들고 인증·제한·모니터링을 제공하는 API 프록시 서비스

  ### (AWS) AppSync
  > GraphQL 기반 API를 만들고 실시간·오프라인 동기화를 제공하는 서버리스 GraphQL 서비스

  ### Route53
  > DNS 레코드 관리와 헬스체크, 지능형 라우팅을 제공하는 클라우드 DNS 서비스

  ### 글로벌 액셀레이터
  > AWS 글로벌 네트워크를 통해 트래픽을 최적 경로로 전달해 지연 시간과 가용성을 개선하는 서비스

  ### (AWS) Outposts
  > AWS 인프라와 서비스를 온프레미스에 설치해 하이브리드 클라우드를 구성하는 서비스

  ### (AWS) WaveLength
  > 통신사 5G 엣지 로케이션에서 초저지연 애플리케이션을 실행할 수 있게 하는 서비스

  ### (AWS) LocalZones
  > 특정 도시 근처에 컴퓨팅 리소스를 배치해 최종 사용자와의 지연 시간을 줄이는 로컬 리전 확장

## 6.스토리지

  ### (Amazon) EFS
  > 여러 EC2 인스턴스에서 동시에 마운트 가능한 탄력적 NFS 파일 스토리지

  ### (Amazon) S3
  > 대용량 객체를 안전하게 저장하고 버전 관리·수명주기 정책을 제공하는 객체 스토리지

  ### (Amazon) Fsx
  > Windows, NetApp, Lustre 등 특수 파일시스템을 관리형으로 제공하는 고성능 파일 스토리지

  ### (AWS) DataSync
  > 온프레미스와 AWS 스토리지 간 대규모 데이터를 빠르고 안전하게 전송·동기화하는 서비스

## 7.캐싱

  ### CloudFront
  > 전 세계 엣지 로케이션에서 콘텐츠를 캐싱해 빠르게 전송하는 CDN 서비스

  ### Lambda Edge
  > CloudFront 엣지 위치에서 요청·응답을 가공하는 서버리스 함수 실행 기능

  ### (Amazon) ElasticCache
  > Redis 또는 Memcached 기반 인메모리 캐시를 관리형으로 제공하는 서비스

## 8.데이터베이스

  ### DynamoDB
  > 완전관리형 NoSQL 키-값/문서 데이터베이스로, 초당 대량 트래픽을 자동 스케일링으로 처리

  ### (Amazon) OpenSearch
  > 검색, 로그 분석, 관측 데이터를 위한 관리형 OpenSearch/Elasticsearch 서비스

  ### RDS
  > MySQL, PostgreSQL, Oracle 등 관계형 데이터베이스를 백업·패치 포함 관리형으로 제공하는 서비스

  ### Aurora
  > MySQL·PostgreSQL 호환의 고성능·고가용성 관리형 관계형 데이터베이스

## 9.서비스통신

  ### Step Function
  > 여러 Lambda·서비스 호출을 상태 머신으로 정의해 워크플로우를 오케스트레이션하는 서비스

  ### SQS
  > 메시지를 비동기로 저장해 마이크로서비스 간 결합도를 낮추는 큐 서비스

  ### (Amazon) MQ
  > ActiveMQ/RabbitMQ 기반 관리형 메시지 브로커 서비스

  ### (Amazon) SNS
  > 여러 구독자에게 동시에 메시지를 팬아웃하는 발행/구독 메시징 서비스

## 10.데이터 엔지니어링

  ### Kinesis Data Streams
  > 대량의 스트리밍 데이터를 실시간으로 수집·처리하기 위한 데이터 스트림 서비스

  ### Kinesis Data Firehose
  > 스트리밍 데이터를 S3, Redshift, OpenSearch 등 대상으로 자동 적재하는 서비스

  ### Kinesis Data Anaytics
  > 스트리밍 데이터에 대해 SQL 또는 애플리케이션으로 실시간 분석을 수행하는 서비스

  ### (Amazon) MSK
  > Apache Kafka 클러스터를 완전관리형으로 제공하는 스트리밍 플랫폼

  ### (AWS) Batch
  > 대규모 배치 컴퓨팅 작업을 자동으로 스케줄링·스케일링해 실행하는 서비스

  ### (Amazon) EMR
  > Hadoop, Spark 등 빅데이터 프레임워크를 관리형 클러스터로 제공하는 분석 플랫폼

  ### (AWS) Glue
  > ETL 작업과 데이터 카탈로그를 제공하는 서버리스 데이터 통합 서비스

  ### Redshift
  > 대규모 분석 쿼리를 위한 컬럼 기반 데이터 웨어하우스 서비스

  ### (Amazon) DocumentDB
  > MongoDB 호환 문서형 데이터베이스를 관리형으로 제공하는 서비스

  ### (Amazon) Timestream
  > IoT, 모니터링 데이터에 최적화된 시계열 데이터베이스 서비스

  ### (Amazon) Athena
  > S3에 저장된 데이터를 서버리스로 바로 SQL 쿼리할 수 있는 대화형 쿼리 서비스

  ### (Amazon) Quick Sight
  > 대시보드와 시각화를 제공하는 서버리스 BI(비즈니스 인텔리전스) 서비스

## 11.모니터링

  ### CloudWatch
  > 로그·메트릭·알람을 통해 리소스와 애플리케이션을 모니터링하는 통합 관측 서비스

  ### EventBridge
  > SaaS, AWS 서비스, 자체 애플리케이션 이벤트를 라우팅하는 서버리스 이벤트 버스

  ### X-Ray
  > 분산 애플리케이션의 요청 경로를 추적해 성능 병목과 오류를 분석하는 서비스

## 12.배포 및 인스턴스 관리

  ### Elastic Beanstalk
  > 애플리케이션 코드만 업로드하면 인프라 프로비저닝과 배포를 자동으로 해주는 PaaS

  ### CodeDeploy
  > EC2, 온프레미스, Lambda 등에 애플리케이션을 자동 배포하고 롤백을 지원하는 서비스

  ### CloudFormation
  > 인프라를 템플릿으로 정의해 생성·수정·삭제하는 코드형 인프라(IaC) 서비스

  ### 서비스 카탈로그
  > 승인된 템플릿·제품 카탈로그를 통해 표준화된 인프라를 배포하게 해주는 서비스

  ### 서버리스 애플리케이션 모딜(SAM)
  > CloudFormation 확장을 이용해 서버리스 애플리케이션을 쉽게 정의·배포하는 프레임워크

  ### (AWS) 클라우드 개발 키드(CDK)
  > 프로그래밍 언어로 인프라를 정의하고 CloudFormation 템플릿으로 변환해 배포하는 IaC 도구

  ### (AWS) Systems Manager(SSM)
  > 패치, 파라미터, Run Command 등 인스턴스를 중앙에서 운영·관리하게 해주는 서비스 모음

  ### (AWS) Cloud Map
  > 서비스 디스커버리와 헬스체크를 제공해 마이크로서비스 위치를 동적으로 관리하는 서비스

## 13.비용제어

  ### (AWS) 태그(Tag)
  > 리소스에 키/값 메타데이터를 붙여 비용, 책임부서, 환경 등을 구분·관리하게 해주는 기능

  ### Trusted Advisor
  > 비용, 보안, 성능, 내결함성 모범 사례 기준으로 계정을 자동 점검하는 권장사항 서비스

  ### (AWS) Service Quotas
  > 각 서비스별 사용 한도(quota)를 조회·요청·관리하는 서비스

  ### (AWS) Budgets Cost Explorer
  > 예산을 설정하고 사용량·비용 추세를 분석해 초과 시 알림을 주는 비용 관리 도구

  ### (AWS) Compute Optimizer
  > 사용 패턴을 분석해 EC2, Lambda 등의 인스턴스 크기 최적화를 추천해 주는 서비스

## 14.마이그레이션(Migration)

  ### Storage Gateway
  > 온프레미스에서 AWS 스토리지를 로컬 스토리지처럼 사용하게 해주는 하이브리드 스토리지 게이트웨이

  ### (AWS) Snow Family
  > 대용량 데이터를 오프라인 장비를 통해 AWS로 옮기는 데이터 전송 장비 제품군

  ### Database Migration Service(DMS)
  > 서로 다른 데이터베이스 간에 최소 다운타임으로 데이터를 마이그레이션하는 서비스

  ### 클리우드 도입 준비 도구 (CART)
  > 조직의 클라우드 도입 준비 상태를 평가하는 진단·평가 도구

  ### VM migrations Services
  > 온프레미스 또는 타 클라우드의 VM을 AWS로 이전하는 마이그레이션 서비스

  ### (AWS) Backup
  > 여러 서비스의 백업 정책을 중앙에서 정의하고 자동 백업·복구를 제공하는 서비스

## 15.VPC

  ### VPC
  > 격리된 가상 네트워크를 구성해 서브넷, 라우팅, 보안 그룹 등을 제어하는 네트워크 서비스

  ### Transit GateWay
  > 여러 VPC와 온프레미스 네트워크를 허브-스포크 구조로 연결해 라우팅을 단순화하는 서비스

  ### 엔드 포인트
  > 인터넷을 거치지 않고 AWS 서비스에 비공개 네트워크로 접속하게 해주는 VPC 엔드포인트 기능

  ### PrivateLink
  > 다른 계정·서비스를 VPC 엔드포인트 형태로 프라이빗하게 노출하는 서비스

  ### (AWS) S2S VPN
  > 온프레미스 네트워크와 VPC를 IPsec 터널로 연결하는 사이트 간 VPN 서비스

  ### (AWS) Client VPN
  > 사용자가 각자 디바이스에서 VPC로 접속하는 관리형 클라이언트 VPN 서비스

  ### Direct Connect
  > 온프레미스 데이터센터와 AWS를 전용 회선으로 저지연·안정적으로 연결하는 서비스

## 16.머신러닝

  ### Rekognition
  > 이미지와 동영상에서 객체, 얼굴, 텍스트 등을 분석하는 컴퓨터 비전 서비스

  ### Transcribe
  > 음성을 텍스트로 변환하는 자동 음성 인식 서비스

  ### Polly
  > 텍스트를 자연스러운 음성으로 변환하는 TTS(텍스트-음성 변환) 서비스

  ### Translate
  > 여러 언어 간 텍스트를 자동 번역하는 기계 번역 서비스

  ### (Amazon) Lex
  > 음성·텍스트 기반 챗봇을 만드는 자연어 이해(NLU) 서비스

  ### (Amazon) Connect
  > 클라우드 기반 콜센터를 빠르게 구축할 수 있는 컨택 센터 서비스

  ### Comprehend
  > 텍스트에서 감정, 엔티티, 키워드 등을 추출하는 자연어 처리(NLP) 서비스

  ### SageMaker
  > 머신러닝 모델을 구축·학습·튜닝·배포하는 통합 ML 플랫폼

  ### Forcast
  > 시계열 데이터를 이용해 수요 예측 등을 수행하는 예측 분석 서비스

  ### Kendra
  > 엔터프라이즈 문서들을 대상으로 고품질 검색을 제공하는 지능형 검색 서비스

  ### Personalize
  > 사용자의 행동 데이터를 기반으로 개인화 추천 기능을 쉽게 구현하게 해주는 서비스

  ### Textract
  > 스캔 문서에서 텍스트와 테이블·폼 구조를 자동 추출하는 OCR 서비스

## 17.기타서비스

  ### CodeCommit
  > Git 기반 소스 코드를 호스팅하는 완전관리형 버전 관리 서비스

  ### (Amazon) CodeGuru
  > 코드 품질과 성능을 자동으로 리뷰하고 개선점을 제안하는 AI 기반 도구

  ### Kinesis Video Streams
  > 대규모 비디오 스트림을 AWS로 수집·저장·처리하는 서비스

  ### (AWS) WorkSpaces
  > 클라우드에서 제공되는 가상 데스크톱(VDI)을 제공하는 서비스

  ### (Amazon) AppStream 2.0
  > 데스크톱 애플리케이션을 브라우저로 스트리밍해 제공하는 서비스

  ### (AWS) Device Farm
  > 실제 모바일 기기와 브라우저에서 앱을 자동 테스트하는 서비스

  ### (Amazon) Macie
  > S3에 저장된 민감한 데이터를 자동 탐지·분류해 데이터 보안을 돕는 서비스

  ### (Amazon) SES
  > 대량 이메일 발송과 수신을 위한 확장 가능한 이메일 서비스

  ### (Amazon) Pinpoint
  > 이메일, 푸시, SMS 등 멀티채널 고객 참여(캠페인·마케팅)를 관리하는 서비스
