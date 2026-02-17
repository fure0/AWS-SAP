### 🔐 AssumeRole 이란?

AssumeRole은 Amazon Web Services 의 IAM 기능 중 하나로,
다른 IAM 역할(Role)의 권한을 일시적으로 빌려 사용하는 것을 말합니다.


### 🔐 IdP 란?

IdP (Identity Provider) 는 사용자의 신원을 인증(로그인 확인)해주는 주체입니다.
즉,“이 사람이 누구인지”를 확인해주는 시스템이에요.

### 📌 AWS 문맥에서의 IdP

Amazon Web Services 에서는 외부 인증 시스템을 통해 로그인할 수 있도록 지원합니다.

예를 들어:
회사 계정으로 AWS 콘솔 로그인
Google 계정으로 로그인
Okta로 로그인
이때 그 인증을 담당하는 것이 IdP


### 🔑 개념 구분
개념	의미
IdP	: 인증 담당 (너 누구야?)
AWS : IAM	권한 담당 (뭐 할 수 있어?)
AssumeRole : 인증 후 권한 위임



### 1️⃣ RI (Reserved Instances)
특정 인스턴스를 1년 또는 3년 약정해서 할인받는 방식

### 2️⃣ Savings Plans
“이 인스턴스를 쓰겠다”가 아니라 “시간당 얼마만큼 쓰겠다”를 약정

### 🆚 RI vs Savings Plans 비교
| 항목     | RI           | Savings Plan           |
| ------ | ------------ | ---------------------- |
| 유연성    | 낮음           | 높음                     |
| 관리 복잡도 | 높음           | 낮음                     |
| 서비스 범위 | EC2 중심       | EC2 + Lambda + Fargate |
| 추천 상황  | 매우 고정적인 워크로드 | 일반적인 대부분의 경우           |

실무 결론
현재 AWS에서는 👉 Savings Plans가 거의 기본 선택지