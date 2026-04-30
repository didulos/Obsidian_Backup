---
type: term
category: [MLOps, Infra]
status: seed

---

## 정의

Docker는 애플리케이션을 컨테이너(container)라는 경량의 독립적 환경에 패키징하여 어디서나 동일하게 실행할 수 있도록 하는 컨테이너화(containerization) 플랫폼이다. 개발 환경, 테스트 환경, 프로덕션 환경 간의 일관성을 보장하여 "내 로컬에서는 되는데"라는 문제를 해결한다.

## 왜 중요한가

ML/AI 프로젝트에서 모델 서빙(serving)과 배포(deployment) 시 의존성 관리, 환경 일관성, 확장성을 동시에 보장하므로 필수 도구이다. 특히 데이터 파이프라인과 모델 인퍼런스(inference) 환경을 재현 가능하게 만든다.

## 관련 개념

- 상위 개념: [[Virtualization]](가상화)

- 하위 개념: [[Image]](이미지), [[Container]](컨테이너)

- 연관 개념: [[Kubernetes]](쿠버네티스), [[CI/CD]](지속적 통합/배포), [[Model-Serving]](모델 서빙)

## 비유로 이해하기

Docker는 레고 블록처럼 생각할 수 있다. 각 애플리케이션이 담긴 컨테이너는 독립적인 레고 블록이며, 어느 컴퓨터(기지판)에 올려놔도 같은 모양으로 동작한다.

## 실제 사용 예시

```
FROM python:3.9
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
CMD ["python", "app.py"]
```

위 Dockerfile을 빌드하면 Python 애플리케이션이 항상 동일한 환경에서 실행되는 이미지가 생성되고, 이를 어느 서버에서도 컨테이너로 실행할 수 있다.