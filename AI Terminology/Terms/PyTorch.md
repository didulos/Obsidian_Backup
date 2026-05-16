---
type: term
category: [Deep-Learning, MLOps]
status: seed

---

## 정의

PyTorch는 페이스북(현 메타)에서 개발한 오픈소스 머신러닝 프레임워크(framework)로, 동적 계산 그래프(dynamic computational graph)를 기반으로 신경망을 구축하고 훈련할 수 있게 해준다. 파이썬 친화적인 API를 제공하여 연구와 프로덕션 환경에서 모두 널리 사용된다.

## 왜 중요한가

PyTorch는 직관적인 문법과 강력한 자동미분(automatic differentiation) 기능으로 딥러닝 모델 개발 생산성을 크게 향상시킨다. 현재 학계와 산업계에서 가장 인기 있는 딥러닝 프레임워크로, 최신 AI 모델 구현에 필수적인 도구다.

## 관련 개념

- 상위 개념: [[Deep-Learning]](딥러닝)

- 하위 개념: [[Tensor]](텐서), [[Autograd]](자동미분)

- 연관 개념: [[Neural-Network]](신경망), [[GPU-Computing]](GPU 컴퓨팅), [[Model-Training]](모델 훈련)

## 비유로 이해하기

PyTorch는 레고 블록처럼 기본 단위(텐서, 레이어)를 조립하여 복잡한 신경망 구조를 유연하게 만들 수 있는 도구다. 필요에 따라 블록을 자유롭게 변형하고 재조합할 수 있다.

## 실제 사용 예시

```python
import torch
import torch.nn as nn

# 간단한 신경망 정의
model = nn.Sequential(
    nn.Linear(784, 128),
    nn.ReLU(),
    nn.Linear(128, 10)
)

# 텐서 생성 및 순전파
x = torch.randn(32, 784)
output = model(x)
```