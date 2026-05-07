---
title: "Embedding이란?"
date: 2026-05-07
created: 2026-05-07T08:58:07
tags: [qa, embedding, vector-search, machine-learning]
topic: embedding
related:
  - "[[2026-05-07-data-log-qa-definition]]"
source: claude-opus-4-7
status: archived
---

# Embedding이란?

## Ask & Output

**Ask:**
Embedding이란 무엇이며 어떤 경우에 쓰이나

**Output:**
Embedding은 이산적이거나 고차원의 데이터(텍스트·이미지·카테고리 등)를 의미를 보존한 채 저차원의 연속적인 벡터 공간으로 변환한 표현이다. 핵심 원리는 "비슷한 것은 가까이, 다른 것은 멀리" 배치하는 것으로, 벡터 거리(코사인 유사도 등)로 의미적 유사성을 계산할 수 있게 한다. 주된 활용처는 의미 기반 검색, RAG, 추천 시스템, 클러스터링/이상치 탐지, 중복 검출, 멀티모달 검색 등이며, 비슷한 것을 빠르게 찾아야 하는 거의 모든 문제에서 1차 후보다.

## Lessons Learned

- Embedding의 본질은 "단어/이미지를 숫자로 바꾸는 변환"이 아니라, **의미적 유사성을 거리로 환산할 수 있는 좌표계로 매핑하는 것**이다 — 즉 핵심은 변환 자체가 아니라 "거리=의미 유사도"라는 성질이 보존된다는 점.
- 텍스트와 이미지를 **같은 벡터 공간**에 매핑하는 멀티모달 embedding(CLIP 등)이 존재하기 때문에, "텍스트로 이미지 검색", "이미지로 비슷한 이미지 검색"이 본질적으로 같은 연산(벡터 거리 계산)으로 통합된다.

## Better Ask

**Before:**
Embedding이란 무엇이며 어떤 경우에 쓰이나

**After:**
ML/AI 입문자 관점에서 embedding이 무엇인지 직관적으로 설명해줘. (1) 어떤 종류의 데이터를 어떤 형태로 변환하는지, (2) 변환 후 실제로 어떻게 활용하는지(거리 계산·검색 등), (3) 대표적인 실무 활용 사례(RAG·추천·검색 등)를 카테고리별로 정리해줘. 코드 예시는 필요 없고 개념 이해가 우선이야.

---

*Related: [[2026-05-07-data-log-qa-definition]]*
