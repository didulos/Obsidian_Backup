---

type: term

category: [Machine-Learning, Deep-Learning]

status: seed

---

## 정의

데이터나 모델에서 대부분의 값이 0이거나 무의미하고, 소수의 값만 의미 있는 상태를 의미한다. 스파스 데이터(sparse data)는 벡터나 행렬의 대부분 원소가 0이며, 스파스 모델(sparse model)은 많은 가중치(weight)가 0에 가깝거나 정확히 0인 상태를 말한다.

## 왜 중요한가

스파스 구조를 활용하면 메모리 사용량과 계산 비용을 대폭 줄일 수 있으며, 모델의 해석가능성(interpretability)을 높인다. 특히 텍스트나 추천 시스템 같은 고차원 데이터에서 효율적인 처리를 가능하게 한다.

## 관련 개념

- 상위 개념: [[Data-Representation]](데이터 표현)

- 하위 개념: [[One-Hot-Encoding]](원-핫 인코딩), [[Bag-of-Words]](단어 주머니)

- 연관 개념: [[Regularization]](정규화), [[Feature-Selection]](특성 선택), [[Dimensionality-Reduction]](차원 축소)

## 비유로 이해하기

도시의 아파트 주소록처럼, 대부분의 칸은 비어있지만 실제 거주자 정보만 기록된 것과 같다. 불필요한 정보를 저장하지 않아 공간을 절약한다.

## 실제 사용 예시

텍스트 분류에서 단어 등장 여부를 표현한 벡터는 대부분 0이고 특정 단어만 1인 스파스 데이터다. L1 정규화(regularization)를 적용하면 많은 가중치를 0으로 만들어 스파스 모델을 만들 수 있다.