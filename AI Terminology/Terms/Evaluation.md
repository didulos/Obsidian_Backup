---
type: term
category: [Machine-Learning, MLOps]
status: seed

---

## 정의

모델의 성능을 측정하고 검증하는 과정으로, 학습된 모델이 새로운 데이터에 대해 얼마나 잘 작동하는지 판단하는 단계이다. 정확도(accuracy), 정밀도(precision), 재현율(recall) 등 다양한 지표(metric)를 통해 모델의 강점과 약점을 파악한다.

## 왜 중요한가

모델의 과적합(overfitting) 여부를 판단하고, 실제 프로덕션 환경에서의 성능을 예측할 수 있기 때문에 필수적이다. 평가 없이는 모델 개선 방향을 결정할 수 없다.

## 관련 개념

- 상위 개념: [[Model-Development]](모델 개발)

- 하위 개념: [[Cross-Validation]](교차 검증), [[A-B-Testing]](A/B 테스트)

- 연관 개념: [[Metrics]](평가 지표), [[Validation]](검증), [[Test-Set]](테스트 셋)

## 비유로 이해하기

학생이 시험을 치르기 전에 모의고사로 자신의 실력을 확인하는 것처럼, 모델도 실제 배포 전에 평가를 통해 성능을 검증해야 한다.

## 실제 사용 예시

이진 분류 모델의 평가에서 정밀도 95%, 재현율 87%를 얻었다면, 거짓 양성(false positive)은 적지만 거짓 음성(false negative)이 많다는 의미이므로 비즈니스 요구사항에 맞춰 임계값(threshold)을 조정해야 한다.