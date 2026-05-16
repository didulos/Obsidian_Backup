---
type: term

category: [MLOps, Infra]

status: seed

---

## 정의

Advanced Package Tool(APT)은 리눅스 기반 시스템에서 소프트웨어 패키지의 설치, 업데이트, 제거를 자동으로 관리하는 패키지 관리자(package manager)이다. 주로 Debian, Ubuntu 등의 리눅스 배포판에서 사용되며, 패키지 간의 의존성(dependency)을 자동으로 해결해준다.

## 왜 중요한가

AI/ML 프로젝트에서 필요한 라이브러리와 시스템 의존성을 효율적으로 관리할 수 있으며, 환경 설정 시간을 단축하고 재현성 있는(reproducible) 개발 환경을 구축하는 데 필수적이다.

## 관련 개념

- 상위 개념: [[Package-Manager]](패키지 관리자)

- 하위 개념: [[apt-get]](apt-get 명령어), [[dpkg]](Debian 패키지)

- 연관 개념: [[Docker]](도커), [[pip]](Python 패키지 관리자), [[conda]](Conda 패키지 관리자)

## 비유로 이해하기

음식점의 식재료 공급업체처럼, APT는 필요한 소프트웨어와 그 재료(의존성)를 한 번에 주문하고 배송해주는 역할을 한다.

## 실제 사용 예시

```
apt-get update  # 패키지 목록 최신화
apt-get install python3-dev  # Python 개발 도구 설치
```