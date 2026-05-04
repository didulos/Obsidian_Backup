---
type: term
category: [Data-Engineering]
status: seed

---

## 정의

ELT(Extract, Load, Transform)는 원본 데이터를 먼저 목표 시스템으로 적재한 후, 그 안에서 변환 작업을 수행하는 데이터 파이프라인 패턴이다. 전통적인 [[ETL]](Extract, Transform, Load)과 달리 변환 순서가 뒤바뀐 방식으로, 클라우드 기반 데이터 웨어하우스의 확산으로 인기가 높아졌다.

## 왜 중요한가

현대적인 클라우드 인프라에서는 원본 데이터를 빠르게 저장하고 나중에 필요에 따라 변환하는 ELT 방식이 더 효율적이고 유연하다. 스케일 가능한 컴퓨팅 환경에서 대용량 데이터 처리를 간소화할 수 있기 때문이다.

## 관련 개념

- 상위 개념: [[Data-Pipeline]](데이터 파이프라인)
- 하위 개념: [[Incremental-Load]](증분 적재), [[Reverse-ETL]](역 ETL)
- 연관 개념: [[Data-Warehouse]](데이터 웨어하우스), [[dbt]](dbt), [[Apache-Airflow]](Apache Airflow)

## 비유로 이해하기

사진을 정렬하고 편집하는 과정으로, ELT는 먼저 모든 사진을 폴더에 저장한 후 클라우드에서 필요에 따라 편집하는 것이고, ETL은 편집을 먼저 마친 후 저장하는 것과 같다.

## 실제 사용 예시

Snowflake나 BigQuery 같은 클라우드 데이터 웨어하우스에서 원본 데이터를 스테이징 테이블로 로드한 후, SQL을 이용해 비즈니스 로직에 맞게 변환하여 분석 테이블을 만든다.