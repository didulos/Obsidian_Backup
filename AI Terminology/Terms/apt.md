---
type: term
category: [Machine-Learning]
status: seed

---

## 정의

적응형 확률 테이블(Adaptive Probability Table)의 약자로, 머신러닝 모델이 학습 과정에서 예측 오류에 기반하여 동적으로 확률 분포를 조정하는 메커니즘이다. 주로 온라인 학습(online learning)이나 강화학습(reinforcement learning) 환경에서 모델의 성능을 개선하는 데 사용된다.

## 왜 중요한가

실무에서 데이터 분포가 시간에 따라 변하는 상황(concept drift)에서 모델이 지속적으로 적응할 수 있도록 해주므로, 특히 추천 시스템이나 이상 탐지 같은 동적 환경에서 모델의 신뢰도를 유지하는 데 필수적이다.

## 관련 개념

- 상위 개념: [[Machine-Learning]](머신러닝)
- 하위 개념: [[Online-Learning]](온라인 학습), [[Concept-Drift]](개념 드리프트)
- 연관 개념: [[Reinforcement-Learning]](강화학습), [[Bayesian-Update]](베이지안 업데이트), [[Adaptive-Algorithm]](적응형 알고리즘)

## 비유로 이해하기

날씨가 자주 바뀌는 지역의 일기예보사가 매일의 실제 날씨를 관찰하며 자신의 예측 모델을 조정하는 것처럼, apt는 새로운 데이터를 보며 실시간으로 확률 분포를 갱신한다.

## 실제 사용 예시

추천 시스템에서 사용자의 선호도 변화를 감지하여 확률 테이블을 매일 업데이트하거나, 이상 탐지 모델이 새로운 패턴의 공격을 학습하면서 정상/비정상 경계값을 자동으로 재조정하는 경우에 사용된다.