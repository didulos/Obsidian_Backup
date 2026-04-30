---
type: term
category: [Deep-Learning, Machine-Learning]
status: seed

---

## 정의

신경망(neural network)의 여러 계층(layer)을 깊게 쌓아 복잡한 패턴을 학습하는 머신러닝 방식이다. 입력층에서 출력층까지 다중의 은닉층(hidden layer)을 통과하면서 데이터의 고수준 표현(high-level representation)을 자동으로 추출한다.

## 왜 중요한가

이미지, 음성, 텍스트 등 비정형 데이터에서 수작업 없이 특징을 자동 추출할 수 있어 현대 AI의 핵심 기술이다. [[Transformer]](트랜스포머)와 결합하여 [[LLM]](대형언어모델) 등 최신 AI 모델의 기반을 이룬다.

## 관련 개념

- 상위 개념: [[Machine-Learning]](머신러닝)

- 하위 개념: [[Convolutional-Neural-Network]](합성곱신경망), [[Recurrent-Neural-Network]](순환신경망)

- 연관 개념: [[Backpropagation]](역전파), [[Gradient-Descent]](경사하강법), [[Activation-Function]](활성화함수)

## 비유로 이해하기

마치 책을 읽을 때 글자 → 단어 → 문장 → 의미 순으로 단계적으로 이해하는 것처럼, 딥러닝도 낮은 수준의 특징(엣지, 색상)부터 시작해 점차 높은 수준의 개념(얼굴, 객체)으로 추상화해간다.

## 실제 사용 예시

이미지 분류(예: 고양이 vs 개 판별)에서 필터를 수동으로 설계하지 않고도 네트워크가 자동으로 학습한다. ChatGPT, DALL-E 같은 생성형 AI도 수십억 개의 파라미터(parameter)를 가진 깊은 신경망으로 구동된다.