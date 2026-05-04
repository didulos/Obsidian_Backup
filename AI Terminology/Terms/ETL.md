---
type: term
category: [Data-Engineering]
status: seed

---

## 정의

ETL은 데이터를 원본 시스템에서 추출(Extract)하고, 변환(Transform)한 후, 목표 시스템에 적재(Load)하는 데이터 파이프라인(data pipeline) 프로세스다. 데이터 품질 관리와 통합을 위한 핵심 기술이다.

## 왜 중요한가

서로 다른 데이터 소스(data source)의 데이터를 통합하여 분석 가능한 형태로 만들어야 하는 모든 데이터 기반 조직에 필수적이다. 데이터 거버넌스(data governance)와 품질 관리의 기초를 제공한다.

## 관련 개념

- 상위 개념: [[Data-Integration]](데이터 통합)

- 하위 개념: [[ELT]](역순 로드), [[Data-Pipeline]](데이터 파이프라인)

- 연관 개념: [[Data-Warehouse]](데이터 웨어하우스), [[Data-Quality]](데이터 품질), [[Data-Orchestration]](데이터 오케스트레이션)

## 비유로 이해하기

음식 재료를 여러 공급처에서 받아 세척(추출)하고, 손질해서 규격에 맞게 준비(변환)한 후, 냉동고에 보관(적재)하는 과정과 같다.

## 실제 사용 예시

온라인 쇼핑몰의 웹 로그, 결제 DB, 재고 시스템에서 데이터를 추출해 날짜 형식을 통일하고 이상값을 제거한 후 데이터 웨어하우스에 저장하는 경우. Apache Airflow나 Talend 같은 도구로 매일 자동화된 ETL 작업을 실행한다.