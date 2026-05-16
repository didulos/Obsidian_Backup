---
type: term

category: [MLOps, Infra]

status: seed

---

## 정의

Python 패키지 관리자(package manager)로, 파이썬 프로젝트에 필요한 라이브러리를 PyPI(Python Package Index) 저장소에서 다운로드하여 설치하고 관리하는 도구이다. 의존성(dependency) 관리를 자동화하여 개발 환경 구성을 단순화한다.

## 왜 중요한가

머신러닝 프로젝트에서 [[Pandas]](판다스), [[NumPy]](넘파이), [[scikit-learn]] 등 수많은 라이브러리를 효율적으로 관리할 수 있으며, 버전 호환성 문제를 체계적으로 해결할 수 있다. 재현 가능한(reproducible) 개발 환경 구축에 필수적이다.

## 관련 개념

- 상위 개념: [[Package-Manager]](패키지 관리자)

- 하위 개념: [[virtual-environment]](가상 환경), [[requirements.txt]](의존성 명시 파일)

- 연관 개념: [[Conda]](콘다), [[Docker]](도커), [[Git]](깃)

## 비유로 이해하기

요리에 필요한 재료를 마트에서 사는 것처럼, pip는 파이썬 프로젝트에 필요한 라이브러리들을 PyPI 온라인 저장소에서 자동으로 찾아서 설치해주는 장보기 도우미다.

## 실제 사용 예시

`pip install numpy==1.21.0`으로 특정 버전의 넘파이를 설치하거나, `pip install -r requirements.txt`로 프로젝트 전체 의존성을 한 번에 설치할 수 있다.