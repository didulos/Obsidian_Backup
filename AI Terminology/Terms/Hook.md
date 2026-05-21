---

type: term

category: [Deep-Learning, MLOps]

status: seed

---

## 정의

hook은 프로그램 실행 흐름의 특정 지점에서 자동으로 실행되는 콜백 함수(callback function)이다. 딥러닝 프레임워크에서는 학습(training), 검증(validation), 추론(inference) 단계의 전후에 사용자 정의 로직을 삽입하는 메커니즘으로 사용된다. 주로 모니터링, 조기 종료(early stopping), 체크포인트 저장 등을 구현하는 데 활용된다.

## 왜 중요한가

hook을 통해 학습 루프를 직접 수정하지 않으면서도 커스텀 동작을 추가할 수 있어, 코드의 재사용성과 유지보수성을 크게 높인다. 특히 복잡한 학습 파이프라인에서 실험(experiment) 관리와 모델 최적화를 효율적으로 수행할 수 있게 한다.

## 관련 개념

- 상위 개념: [[Callback]](콜백)

- 하위 개념: [[Early-Stopping]](조기 종료), [[Checkpoint]](체크포인트)

- 연관 개념: [[Training-Loop]](훈련 루프), [[Logging]](로깅), [[Metric]](지표)

## 비유로 이해하기

hook은 자동 세차기의 센서와 같다. 차량이 특정 위치에 도달하면 자동으로 세제를 분사하거나 브러시를 작동시키는 것처럼, 모델 학습이 특정 단계(에포크 종료, 배치 처리 완료)에 도달하면 자동으로 지정된 작업을 수행한다.

## 실제 사용 예시

PyTorch Lightning의 `on_epoch_end` hook을 사용하면 매 에포크가 끝날 때마다 모델 성능을 평가하고 최고 성능 모델을 자동 저장할 수 있다. TensorFlow의 `Callback` 클래스를 상속하여 검증 손실(validation loss)이 증가하면 학습을 중단하는 조기 종료 hook을 구현할 수 있다.