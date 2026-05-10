---

type: term

category: [Deep-Learning]

status: seed

---

## 정의

심층 신경망에서 입력층과 출력층 사이의 중간 계층들(hidden layers)을 의미한다. 깊은 네트워크 구조에서 특징 추출(feature extraction)과 표현 학습(representation learning)을 담당하는 핵심 부분이다.

## 왜 중요한가

깊은 모듈은 계층을 거쳐가면서 저수준의 특징에서 고수준의 추상화된 특징으로 변환하므로, 모델의 표현력과 학습 효율을 크게 결정한다. 실무에서 네트워크 깊이와 구조를 설계할 때 필수적으로 고려해야 하는 요소다.

## 관련 개념

- 상위 개념: [[Neural-Network]](신경망)

- 하위 개념: [[Convolutional-Layer]](합성곱 계층), [[Attention-Module]](어텐션 모듈)

- 연관 개념: [[Backpropagation]](역전파), [[Feature-Extraction]](특징 추출), [[Residual-Connection]](잔차 연결)

## 비유로 이해하기

깊은 모듈은 카메라의 초점을 맞추는 여러 렌즈 단계처럼, 입력 데이터를 점진적으로 정제하고 의미 있는 정보로 변환해나가는 과정이다.

## 실제 사용 예시

ResNet의 residual block들이 깊은 모듈을 구성하며, Vision Transformer의 여러 계층의 self-attention 블록들도 깊은 모듈의 예시다.