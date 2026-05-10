---
type: term
category: [Infra]
status: seed

---

## 정의

Cloudflare는 전 세계 데이터 센터 네트워크를 통해 웹사이트와 애플리케이션에 CDN(Content Delivery Network), DDoS 방어, DNS, SSL/TLS 보안 등을 제공하는 클라우드 인프라 플랫폼이다. 사용자의 요청을 지리적으로 가장 가까운 엣지 서버(edge server)로 라우팅하여 성능을 최적화한다.

## 왜 중요한가

ML/AI 서비스를 배포할 때 모델 서버의 응답 속도를 개선하고, DDoS 공격으로부터 보호하며, 글로벌 사용자에게 낮은 지연시간(latency)으로 API를 제공할 수 있다. 특히 [[MLOps]] 파이프라인에서 모델 추론 엔드포인트의 안정성과 성능을 보장하는 핵심 인프라다.

## 관련 개념

- 상위 개념: [[Cloud-Infrastructure]](클라우드 인프라)
- 하위 개념: [[CDN]](콘텐츠 전송 네트워크), [[Edge-Computing]](엣지 컴퓨팅)
- 연관 개념: [[API-Gateway]](API 게이트웨이), [[Load-Balancing]](로드 밸런싱), [[DDoS-Protection]](DDoS 방어)

## 비유로 이해하기

Cloudflare는 전국에 분포된 편의점 물류 센터 같다. 사용자(고객)의 요청은 가장 가까운 센터에서 처리되므로, 중앙 본사(원본 서버)까지 갈 필요가 없어 빠르고 안전하게 서비스받을 수 있다.

## 실제 사용 예시

ML 모델 추론 API를 Cloudflare를 통해 배포하면, 아시아 사용자의 요청은 아시아 엣지 서버에서 처리되어 레이턴시를 50% 이상 단축할 수 있다. Workers 기능으로 간단한 데이터 전처리 로직도 엣지에서 실행 가능하다.