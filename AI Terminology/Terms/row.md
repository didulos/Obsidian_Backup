---
type: term
category: [Data-Engineering]
status: seed

---

## 정의

표(table)의 가로 방향 데이터 단위로, 여러 개의 열(column)로 구성된 레코드(record)를 의미한다. 데이터베이스나 데이터프레임에서 하나의 관찰값(observation) 또는 샘플(sample)에 해당한다.

## 왜 중요한가

데이터 분석과 머신러닝에서 각 행(row)은 학습 데이터의 기본 단위이므로, 데이터 전처리(data preprocessing)와 모델 학습 시 행의 개수와 품질이 성능을 크게 좌우한다.

## 관련 개념

- 상위 개념: [[Table]](테이블)
- 하위 개념: [[Sample]](샘플), [[Instance]](인스턴스)
- 연관 개념: [[Column]](열), [[DataFrame]](데이터프레임), [[Schema]](스키마)

## 비유로 이해하기

엑셀 스프레드시트에서 가로로 펼쳐진 한 줄이 바로 행(row)이다. 각 칸은 열(column)이고, 한 줄 전체가 하나의 완전한 데이터 단위다.

## 실제 사용 예시

pandas 데이터프레임에서 `df.iloc[0]`은 첫 번째 행을 선택하고, `df.shape[0]`은 전체 행의 개수를 반환한다. SQL에서도 `SELECT * FROM users WHERE age > 25`의 각 결과가 하나의 행(row)을 구성한다.