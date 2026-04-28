GitHub

---
type: term
category: [MLOps, Infra]
status: seed
---

## 정의

소프트웨어 개발 프로젝트를 위한 클라우드 기반 버전 관리 및 협업 플랫폼으로, Git(분산 버전 관리 시스템)을 웹 인터페이스로 제공한다. 코드 저장소(repository) 관리, 변경 이력 추적, 팀 협업 기능을 통합적으로 제공한다.

## 왜 중요한가

ML/AI 프로젝트에서 코드, 학습 스크립트, 설정 파일 등을 체계적으로 관리하고 팀원과 협업하는 기본 인프라다. CI/CD 파이프라인(continuous integration/continuous deployment)과 통합되어 모델 배포 자동화의 핵심 역할을 한다.

## 관련 개념

- 상위 개념: [[Version-Control]](버전 관리)

- 하위 개념: [[Pull-Request]](풀 리퀘스트), [[Branch]](브랜치)

- 연관 개념: [[CI/CD]](지속적 통합/배포), [[Git]](깃), [[MLOps]](머신러닝 운영)

## 비유로 이해하기

GitHub는 Google Docs처럼 여러 사람이 동시에 문서를 편집할 수 있지만, 모든 변경 사항을 시간 순서대로 기록하고 필요하면 이전 버전으로 돌아갈 수 있는 "코드 협업 플랫폼"이다.

## 실제 사용 예시

팀의 ML 엔지니어가 새로운 모델 훈련 코드를 작성한 후 Pull Request를 통해 코드 리뷰를 요청하고, 승인 후 main 브랜치에 병합(merge)하면 자동으로 테스트와 배포가 실행된다.