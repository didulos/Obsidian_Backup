---
type: term
category: [Machine-Learning, MLOps]
status: seed

---

## 정의

머신러닝 모델을 학습하고 평가하기 위해 데이터, 모델, 학습 파이프라인(training pipeline)을 통합하여 관리하는 프레임워크 또는 도구. 실험 재현성(reproducibility)과 프로덕션 배포를 위한 일관된 환경을 제공한다.

## 왜 중요한가

데이터 전처리, 모델 학습, 검증, 배포 전 과정을 자동화하고 체계화하여 개발 시간을 단축하고 오류를 줄인다. 팀 협업 시 일관된 실험 환경을 보장한다.

## 관련 개념

- 상위 개념: [[MLOps]](머신러닝 운영)
- 하위 개념: [[Data-Pipeline]](데이터 파이프라인), [[Model-Registry]](모델 레지스트리)
- 연관 개념: [[Experiment-Tracking]](실험 추적), [[Feature-Store]](피처 저장소), [[CI/CD]](지속적 통합/배포)

## 비유로 이해하기

요리사가 재현성 있는 요리를 만들기 위해 레시피, 재료 관리, 조리 과정을 표준화하는 것처럼, harness는 모델 학습의 모든 단계를 체계적으로 정의하고 관리한다.

## 실제 사용 예시

PyTorch Lightning, TensorFlow Keras API, Hugging Face Transformers 같은 프레임워크들이 학습 루프(training loop)를 harness로 제공하여 개발자가 모델 아키텍처에만 집중하도록 한다. MLflow나 Weights & Biases 같은 도구는 전체 ML harness를 관리하는 플랫폼이다.