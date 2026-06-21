---

type: term

category: [Machine-Learning]

status: seed

---

## 정의

props는 컴포넌트나 함수에 전달되는 입력 파라미터(parameter) 또는 설정값(configuration)을 의미한다. 머신러닝 맥락에서는 모델이나 알고리즘의 하이퍼파라미터(hyperparameter)와 유사하게, 외부에서 지정할 수 있는 속성값을 통칭한다.

## 왜 중요한가

props를 통해 같은 컴포넌트나 모델을 다양한 설정으로 재사용할 수 있으며, 코드의 유연성과 재사용성을 크게 높인다. 실무에서 파이프라인 구성, 모델 학습, 데이터 처리 등 거의 모든 단계에서 props 관리가 필수적이다.

## 관련 개념

- 상위 개념: [[Parameter]](파라미터)

- 하위 개념: [[Hyperparameter]](하이퍼파라미터), [[Configuration]](설정값)

- 연관 개념: [[Argument]](인자), [[Attribute]](속성), [[Config-File]](설정파일)

## 비유로 이해하기

props는 레시피를 만들 때 설정하는 온도, 시간, 양념의 양 같은 것이다. 같은 요리 방법(함수)이라도 props(설정값)에 따라 완전히 다른 결과물이 나온다.

## 실제 사용 예시

```python
model = RandomForest(n_estimators=100, max_depth=10, random_state=42)
# n_estimators, max_depth, random_state 등이 props
```

PyTorch 모델에서 Forward 함수에 여러 props를 전달:
```python
output = model(input_data, training=True, dropout_rate=0.5)
```