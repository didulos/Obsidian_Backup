---
type: term
category: [Data-Engineering]
status: seed

---

## 정의

큐(queue)는 먼저 들어온 데이터가 먼저 나가는 선입선출(FIFO, First-In-First-Out) 방식의 데이터 구조다. 데이터 처리 파이프라인에서 작업들을 순차적으로 관리하고 처리 속도의 차이를 완충하는 역할을 한다.

## 왜 중요한가

분산 시스템에서 비동기 작업 처리와 메시지 전달을 위한 필수 인프라다. 처리 속도가 다른 여러 컴포넌트 간의 부하 조절(load balancing)과 데이터 손실 방지를 가능하게 한다.

## 관련 개념

- 상위 개념: [[Data-Structure]](데이터 구조)

- 하위 개념: [[Priority-Queue]](우선순위 큐), [[Message-Queue]](메시지 큐)

- 연관 개념: [[Stream-Processing]](스트림 처리), [[Event-Driven-Architecture]](이벤트 기반 아키텍처), [[Buffering]](버퍼링)

## 비유로 이해하기

은행 대기줄과 같다. 먼저 온 사람이 먼저 업무를 처리받으며, 새로운 사람은 줄 끝에 서서 대기한다.

## 실제 사용 예시

Kafka나 RabbitMQ 같은 메시지 큐 시스템에서 생산자(producer)가 보낸 데이터를 소비자(consumer)가 순차적으로 처리할 때 큐가 중간 완충 역할을 한다. ML 파이프라인에서 대량의 학습 요청을 작업 큐에 넣고 워커들이 순차적으로 처리하는 방식도 큐의 활용 사례다.