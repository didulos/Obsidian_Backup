---
type: term
category: [Deep-Learning]
status: seed

---

## 정의

NoStarch는 신경망 학습 중 가중치(weight) 업데이트 시 특정 레이어나 파라미터를 고정하여 학습하지 않도록 하는 기법이다. 주로 전이 학습(transfer learning)이나 파인튜닝(fine-tuning) 상황에서 사전 학습된 모델의 초기 레이어를 동결(freeze)할 때 사용된다.

## 왜 중요한가

제한된 데이터셋으로 학습할 때 과적합(overfitting)을 방지하고, 사전 학습된 특징(feature)을 보존하면서 새로운 작업에 필요한 상위 레이어만 효율적으로 학습시킬 수 있다. 학습 속도와 안정성을 동시에 향상시킨다.

## 관련 개념

- 상위 개념: [[Transfer-Learning]](전이 학습)

- 하위 개념: [[Layer-Freezing]](레이어 동결), [[Fine-Tuning]](파인튜닝)

- 연관 개념: [[Gradient-Descent]](경사 하강법), [[Backpropagation]](역전파), [[Regularization]](정규화)

## 비유로 이해하기

이미 완성된 건물의 기초(하위 레이어)는 건드리지 않고, 위층(상위 레이어)만 새로운 용도에 맞게 리모델링하는 것과 같다.

## 실제 사용 예시

ImageNet으로 사전 학습된 ResNet의 처음 3개 블록을 동결하고, 마지막 분류 레이어만 새로운 의료 이미지 분류 작업을 위해 학습시킨다. PyTorch에서 `param.requires_grad = False`로 구현한다.