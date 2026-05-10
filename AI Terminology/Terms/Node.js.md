---
type: term
category: [Infra]
status: seed

---

## 정의

Node.js는 Chrome의 V8 JavaScript 엔진을 기반으로 하는 JavaScript 런타임(runtime) 환경으로, 서버 측에서 JavaScript를 실행할 수 있게 해준다. 비동기 이벤트 기반(event-driven) 아키텍처를 채택하여 높은 동시성(concurrency)을 효율적으로 처리한다.

## 왜 중요한가

기계학습 모델 서빙, 데이터 처리 파이프라인, 그리고 실시간 데이터 애플리케이션 구축 시 가볍고 빠른 백엔드를 제공한다. 특히 [[MLOps]] 환경에서 모델 API 서버로 널리 사용된다.

## 관련 개념

- 상위 개념: [[Runtime-Environment]](런타임 환경)
- 하위 개념: [[NPM]](노드 패키지 매니저), [[Express.js]](익스프레스)
- 연관 개념: [[API]], [[Microservices]](마이크로서비스), [[Docker]](도커)

## 비유로 이해하기

Node.js는 여러 손님의 주문을 한 명의 종업원이 효율적으로 처리하는 카페와 같다. 손님이 음료를 기다리는 동안 다른 손님의 주문을 받고, 음료가 준비되면 자동으로(비동기) 전달하는 방식이다.

## 실제 사용 예시

FastAPI나 Flask 같은 Python 기반 ML 서버와 함께, Node.js는 프론트엔드와 모델 서버를 연결하는 게이트웨이(gateway) 역할을 하거나, TensorFlow.js를 사용해 직접 JavaScript에서 경량 모델을 실행할 수 있다.