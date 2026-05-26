---

type: term

category: [Machine-Learning, MLOps]

status: seed

---

## 정의

머신러닝 모델이 학습 또는 추론 과정에서 생성하는 중간 산출물이나 부산물(artifact)을 의미한다. 여기에는 학습된 모델 가중치(model weights), 체크포인트(checkpoint), 로그(log), 메트릭(metric), 그리고 생성된 예측값이나 임베딩 등이 포함된다. MLOps 맥락에서는 모델 레지스트리(model registry)에 저장되어 버전 관리되는 모든 산출물을 지칭한다.

## 왜 중요한가

아티팩트를 체계적으로 관리하지 않으면 모델 재현성(reproducibility)을 보장할 수 없으며, 실험 추적(experiment tracking)과 모델 배포(deployment)가 불가능해진다. 프로덕션 환경에서 모델의 어느 버전이 어떻게 생성되었는지 추적하는 것은 필수적이다.

## 관련 개념

- 상위 개념: [[MLOps]](머신러닝 운영)

- 하위 개념: [[Model-Registry]](모델 레지스트리), [[Checkpoint]](체크포인트)

- 연관 개념: [[Experiment-Tracking]](실험 추적), [[Model-Versioning]](모델 버전 관리), [[Model-Serialization]](모델 직렬화)

## 비유로 이해하기

아티팩트는 영화 촬영 과정에서 생성되는 모든 결과물(필름, 음성, 특수효과 데이터, 메이킹필름 등)과 같다. 최종 영화도 있지만, 그것을 만드는 과정의 모든 중간 산출물이 다시 재현하고 수정하는 데 필요하다.

## 실제 사용 예시

MLflow에서 모델 학습 후 `model.pkl`, `metrics.json`, `params.yaml` 파일들을 artifact store에 저장하여 추후 모델 복원 및 비교 분석을 수행한다. Docker 컨테이너 이미지, 학습된 가중치 파일, 데이터 전처리 스크립트 등 모두가 재현 가능한 배포를 위한 아티팩트가 된다.