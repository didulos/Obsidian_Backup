---
type: term
category: [Infra]
status: seed

---

## 정의

Rust는 메모리 안전성(memory safety)과 동시성(concurrency)을 보장하면서도 C/C++와 같은 성능을 제공하는 시스템 프로그래밍 언어다. 소유권(ownership) 시스템을 통해 컴파일 타임에 메모리 버그를 방지한다.

## 왜 중요한가

ML 인프라 구축 시 고성능이 필요한 데이터 처리, 모델 서빙, 분산 시스템에서 안정성과 속도를 동시에 확보할 수 있어 업계에서 점점 더 채택되고 있다.

## 관련 개념

- 상위 개념: [[Programming-Language]](프로그래밍 언어)

- 하위 개념: [[Cargo]](카고), [[WebAssembly]](웹어셈블리)

- 연관 개념: [[Python]](파이썬), [[Docker]](도커), [[gRPC]]

## 비유로 이해하기

Rust는 엄격한 보안 검사관처럼, 프로그램이 실행되기 전에 코드를 철저히 검증해서 위험한 메모리 접근이 애초에 일어나지 않도록 막는다.

## 실제 사용 예시

Hugging Face의 Tokenizers 라이브러리는 Rust로 핵심 로직을 작성해 Python 인터페이스보다 10배 이상 빠르다. Polars 데이터프레임도 Rust 기반으로 Pandas보다 훨씬 빠른 데이터 처리를 제공한다.