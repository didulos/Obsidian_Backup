---

type: term

category: [MLOps, Machine-Learning]

status: seed

---

## 정의

모델이나 시스템의 성능을 측정하고 분석하기 위해 실행 중인 프로그램의 동작을 추적하고 데이터를 수집하는 과정이다. 프로파일링(profiling)은 CPU 사용량, 메모리 할당, 실행 시간 등 리소스 사용 패턴을 파악하는 데 중점을 둔다.

## 왜 중요한가

모델 학습과 추론 단계에서 성능 병목(bottleneck)을 식별하고 최적화 기회를 발견하는 데 필수적이다. 프로덕션 환경에서 리소스 효율성을 높이고 비용을 절감할 수 있다.

## 관련 개념

- 상위 개념: [[Optimization]](최적화)

- 하위 개념: [[Memory-Profiling]](메모리 프로파일링), [[Performance-Profiling]](성능 프로파일링)

- 연관 개념: [[Monitoring]](모니터링), [[Benchmarking]](벤치마킹), [[Debugging]](디버깅)

## 비유로 이해하기

자동차의 성능을 개선하기 위해 엔진의 회전수, 연료 소비량, 온도 등을 측정하는 것처럼, 프로파일링은 프로그램의 내부 동작을 세밀하게 관찰하는 것이다.

## 실제 사용 예시

PyTorch 모델 학습 시 `torch.profiler`를 사용하여 각 레이어의 연산 시간을 측정하거나, TensorFlow에서 `tf.profiler`로 GPU 메모리 할당 패턴을 분석하여 배치 크기를 조정한다.