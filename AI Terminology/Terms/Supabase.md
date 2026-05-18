---
type: term

category: [Data-Engineering, Infra]

status: seed

---

## 정의

Supabase는 오픈소스 기반의 Firebase 대체제로, PostgreSQL 데이터베이스를 백엔드로 제공하는 BaaS(Backend-as-a-Service) 플랫폼이다. 실시간 데이터베이스(real-time database), 인증(authentication), 스토리지(storage) 등의 기능을 통합 제공하여 백엔드 개발 없이 애플리케이션을 빠르게 구축할 수 있다.

## 왜 중요한가

프로토타입 개발과 스타트업 환경에서 백엔드 구축 시간을 대폭 단축할 수 있으며, PostgreSQL의 강력한 쿼리 능력과 오픈소스의 투명성을 동시에 확보할 수 있어 확장성 있는 데이터 인프라 구축이 가능하다.

## 관련 개념

- 상위 개념: [[BaaS]](백엔드-애즈-어-서비스)

- 하위 개념: [[PostgreSQL]](포스트그레스큐엘), [[JWT]](JSON Web Token)

- 연관 개념: [[Firebase]](파이어베이스), [[REST-API]](REST API), [[Database]](데이터베이스)

## 비유로 이해하기

Supabase는 직접 요리사를 고용해서 요리하는 대신, 준비된 주방 시설과 기본 재료를 제공받고 요리에만 집중할 수 있는 '공유 주방'과 같다. 필요한 모든 백엔드 인프라가 이미 구축되어 있어 비즈니스 로직 개발에만 집중할 수 있다.

## 실제 사용 예시

React 프로젝트에서 Supabase 클라이언트로 로그인 기능을 구현하거나, 실시간 채팅 데이터를 PostgreSQL에서 직접 구독(subscribe)하여 메시지 업데이트를 즉시 화면에 반영할 수 있다.