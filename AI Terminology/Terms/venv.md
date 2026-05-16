---
type: term

category: [MLOps, Infra]

status: seed

---

## 정의

Python 프로젝트의 의존성(dependency)을 격리하기 위해 독립적인 가상 환경(virtual environment)을 생성하는 Python의 표준 도구이다. venv를 사용하면 프로젝트마다 별도의 패키지 버전을 관리할 수 있으며, 시스템 Python 환경을 오염시키지 않는다.

## 왜 중요한가

데이터 사이언스와 ML 프로젝트에서 여러 프로젝트의 패키지 충돌(dependency conflict)을 방지하고, 재현 가능한(reproducible) 환경을 구축하는 기본 관행이다. 팀 협업 시 동일한 개발 환경을 보장하기 위해 필수적이다.

## 관련 개념

- 상위 개념: [[Dependency-Management]](의존성 관리)

- 하위 개념: [[requirements.txt]](패키지 명세 파일), [[pip]](패키지 설치 도구)

- 연관 개념: [[Docker]](컨테이너 환경), [[Conda]](패키지 환경 관리자), [[Git]](버전 관리)

## 비유로 이해하기

venv는 공유 부엌에서 각 요리사가 자신만의 독립적인 주방을 갖는 것과 같다. 한 요리사가 특정 도구나 재료를 추가해도 다른 요리사의 주방에는 영향을 주지 않는다.

## 실제 사용 예시

```
python -m venv myenv
source myenv/bin/activate  # 활성화
pip install pandas scikit-learn==1.0.0
```