API

---
type: term
category: [Infra]
status: seed
---

## 정의

API(Application Programming Interface)는 서로 다른 소프트웨어 애플리케이션이 통신하고 데이터를 교환하기 위한 규칙과 프로토콜의 집합이다. API는 클라이언트가 서버의 기능을 요청(request)하고 응답(response)을 받을 수 있는 인터페이스를 제공한다.

## 왜 중요한가

ML/AI 시스템을 실무에서 운영할 때 학습된 모델을 웹 서비스나 애플리케이션으로 배포(deploy)하려면 반드시 API를 통해 외부와 통신해야 한다. 또한 데이터 수집, 외부 서비스 연동, 마이크로서비스 아키텍처 구축 등 모든 단계에서 필수적이다.

## 관련 개념

- 상위 개념: [[Software-Architecture]](소프트웨어 아키텍처)
- 하위 개념: [[REST-API]](REST API), [[gRPC]](gRPC)
- 연관 개념: [[Endpoint]](엔드포인트), [[Authentication]](인증), [[Microservice]](마이크로서비스)

## 비유로 이해하기

API는 식당의 메뉴판과 주문 시스템에 비유할 수 있다. 손님(클라이언트)은 메뉴판(API 문서)을 보고 원하는 음식(기능)을 주문(요청)하면 주방(서버)에서 처리하여 음식(응답)을 전달받는다.

## 실제 사용 예시

머신러닝 모델을 Flask로 API 서버로 배포할 때: `POST /predict` 엔드포인트를 통해 입력 데이터를 받아 학습된 모델의 예측 결과를 JSON 형식으로 반환한다. 또는 Google Maps API를 활용하여 위치 기반 데이터를 수집할 수 있다.