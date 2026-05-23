---
type: term
category: [MLOps]
status: seed
---

## 정의

더 이상 사용을 권장하지 않는 기능, API, 라이브러리 버전을 의미한다. Deprecated된 요소는 여전히 작동하지만 향후 버전에서 제거될 예정이다. 개발자에게 대체 방안으로 마이그레이션할 것을 권고하는 상태다.

## 왜 중요한가

프로덕션 환경에서 deprecated 요소에 의존하면 향후 라이브러리 업그레이드 시 코드 전체가 깨질 수 있다. 초기에 이를 인식하고 대체 기능으로 전환하면 기술 부채(technical debt)를 예방할 수 있다.

## 관련 개념

- 상위 개념: [[API]](응용프로그래밍인터페이스)

- 하위 개념: [[Breaking-Change]](호환성 깨짐), [[Backward-Compatibility]](하위호환성)

- 연관 개념: [[Version-Control]](버전관리), [[Migration]](마이그레이션), [[Documentation]](문서화)

## 비유로 이해하기

deprecated는 구식 신용카드와 같다. 아직 사용할 수 있지만 은행에서는 새 카드로 바꾸기를 권고하고 있는 상태다. 무시하고 계속 쓰다 보면 결국 사용 불가능한 날이 온다.

## 실제 사용 예시

TensorFlow에서 `tf.contrib` 모듈이 deprecated되어 `tf.keras`로 마이그레이션하도록 안내했다. Python 라이브러리의 경고 메시지에서 "DeprecationWarning: 이 함수는 다음 버전에서 제거됩니다"라고 표시된다.