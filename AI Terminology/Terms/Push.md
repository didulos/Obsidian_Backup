---
type: term
category: [Deep-Learning, MLOps]
status: seed

---

## 정의

신경망의 역전파(backpropagation) 과정에서 손실 함수(loss function)의 기울기를 입력층 방향으로 전파하는 과정이다. 각 계층의 가중치(weight)를 업데이트하기 위해 필요한 그래디언트(gradient)를 계산하는 핵심 메커니즘이다.

## 왜 중요한가

신경망 훈련의 핵심 동작이므로, push의 효율성과 정확성이 모델의 수렴 속도와 최종 성능을 직접 결정한다. 그래디언트 소실(gradient vanishing)이나 폭발(gradient explosion) 같은 문제를 이해하고 해결하기 위해서는 반드시 알아야 한다.

## 관련 개념

- 상위 개념: [[Backpropagation]](역전파)

- 하위 개념: [[Gradient-Descent]](경사 하강법), [[Chain-Rule]](연쇄 법칙)

- 연관 개념: [[Gradient-Vanishing]](그래디언트 소실), [[Optimizer]](최적화기), [[Weight-Update]](가중치 업데이트)

## 비유로 이해하기

손실을 줄이기 위해 산을 내려가는 등산객이 현재 위치에서의 경사도(기울기)를 재측정하고 다음 발을 디딜 방향을 결정하는 과정과 같다. Push는 그 경사도 정보를 등산로 전체에 전파하는 것이다.

## 실제 사용 예시

PyTorch에서 `loss.backward()`를 호출하면 손실로부터 모든 매개변수에 대한 그래디언트가 역방향으로 계산되며, 이를 통해 옵티마이저가 가중치를 업데이트한다.