---
type: term
category: [Data-Engineering, Machine-Learning]
status: seed

---

## 정의

데이터베이스나 대규모 데이터셋에서 빠른 조회와 검색을 위해 생성된 자료 구조(data structure)이다. 인덱스는 원본 데이터의 위치나 식별자를 가리키는 포인터(pointer)를 유지하여 선형 탐색 대신 로그 시간 복잡도(logarithmic time complexity)로 데이터에 접근할 수 있게 한다.

## 왜 중요한가

머신러닝 파이프라인에서 대규모 데이터를 다룰 때 인덱싱은 데이터 전처리(data preprocessing) 속도를 크게 향상시킨다. 특히 벡터 데이터베이스(vector database)나 임베딩 검색(embedding search)에서 인덱싱 없이는 실시간 추론(inference)이 불가능하다.

## 관련 개념

- 상위 개념: [[Data-Structure]](자료 구조)

- 하위 개념: [[Hash-Index]](해시 인덱스), [[B-Tree-Index]](B-트리 인덱스)

- 연관 개념: [[Vector-Database]](벡터 데이터베이스), [[Query-Optimization]](쿼리 최적화), [[Embedding]](임베딩)

## 비유로 이해하기

책의 색인(index)처럼, 전체 페이지를 다 넘기지 않고도 특정 주제가 어느 페이지에 있는지 빠르게 찾을 수 있다. 인덱스도 마찬가지로 데이터셋 전체를 스캔하지 않고 원하는 데이터의 위치를 빠르게 알려준다.

## 실제 사용 예시

추천 시스템(recommendation system)에서 사용자 임베딩을 벡터 인덱스(vector index)에 저장하면, 유사한 사용자나 아이템을 밀리초 단위로 검색할 수 있다. 또한 SQL 데이터베이스에서 자주 조회되는 열(column)에 인덱스를 생성하면 학습 데이터 로딩 시간을 수십 배 단축할 수 있다.