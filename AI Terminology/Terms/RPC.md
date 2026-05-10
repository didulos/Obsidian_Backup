---
type: term
category: [Infra]
status: seed
---

## 정의

원격 프로시저 호출(Remote Procedure Call)은 네트워크를 통해 다른 컴퓨터에 있는 함수나 프로시저를 마치 로컬에서 호출하는 것처럼 실행하는 통신 프로토콜이다. 클라이언트가 서버의 함수를 호출하면 RPC는 요청을 직렬화(serialization)하여 전송하고, 서버는 이를 실행한 후 결과를 다시 반환한다.

## 왜 중요한가

분산 시스템(distributed system)에서 마이크로서비스 간 통신의 기본 패러다임으로, 블록체인 노드, ML 모델 서빙, 데이터 파이프라인 등에서 필수적인 인프라 기술이다.

## 관련 개념

- 상위 개념: [[IPC]](프로세스 간 통신)

- 하위 개념: [[gRPC]](구글 RPC), [[JSON-RPC]](JSON 기반 RPC)

- 연관 개념: [[REST-API]](RESTful API), [[Microservice]](마이크로서비스), [[Serialization]](직렬화)

## 비유로 이해하기

RPC는 마치 다른 도시의 친구에게 전화로 "내 집의 불을 꺼줄 수 있니?"라고 요청하고, 친구가 실행한 후 결과를 보고받는 것과 같다. 직접 가지 않아도 원격지의 작업을 수행받을 수 있다.

## 실제 사용 예시

Web3 지갑이 블록체인 노드와 통신할 때 `eth_sendTransaction` RPC 호출을 사용하며, ML 모델 서빙 플랫폼(예: Ray Serve)에서도 클라이언트가 원격의 모델 추론 함수를 RPC로 호출한다.