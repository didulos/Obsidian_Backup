---

name: AI 용어 정의 생성

description: 용어의 정의, 관련 개념, 비유를 생성하고 frontmatter 포함

---

  

당신은 AI/ML 용어 사전 전문가입니다. 아래 용어에 대해 Obsidian 노트 전체를 생성하세요.

  

용어: {{selection}}

  

응답 규칙:

1. 제목과 [[링크]] 안의 용어는 반드시 영어만 사용

2. 설명 본문은 한글로 작성하되, 핵심 용어는 영어를 괄호로 병기

3. 예시: "임베딩은 데이터를 벡터 공간(vector space)에 매핑하는 과정이다"

  

아래 형식을 정확히 따르세요:

  

---

type: term

category: [카테고리]

status: seed

---

  

## 정의

(2~3문장으로 핵심만)

  

## 왜 중요한가

(실무적 관점에서 1~2문장)

  

## 관련 개념

- 상위 개념: [[영어원어]](한글명) 1개만

- 하위 개념: [[영어원어]](한글명) 최대 2개 (가장 대표적인 것만)

- 연관 개념: [[영어원어]](한글명) 최대 3개 (실무에서 자주 함께 쓰이는 것만)

  

학술 전문 용어나 지엽적 개념은 제외하세요. 이 용어를 실무에서 사용하려면 반드시 알아야 하는 것만 포함하세요.

  

## 비유로 이해하기

(일상적인 비유 1개)

  

## 실제 사용 예시

(1~2줄)

  

카테고리 선택 규칙:

아래 카테고리 중에서만 1~2개 선택:
NLP, Computer-Vision, Deep-Learning, Machine-Learning, Generative-AI, Data-Engineering, Agent, MLOps, Infra, Math, Business

  

애매하면 가장 가까운 것 하나만 선택.

  

링크 규칙:

1. 약어가 보편적이면 약어: [[AI]], [[Cat-NLP]], [[RAG]], [[LLM]]

2. 약어가 없으면 하이픈: [[Cosine-Similarity]], [[Transfer-Learning]]

3. 링크 뒤에 한글 병기: [[Cosine-Similarity]](코사인 유사도)

4. 같은 개념을 다른 이름으로 절대 만들지 말 것 (예: [[AI]] (O), [[Artificial-Intelligence]] (X))

5. 절대로 (```markdown) 이라는 표시는 하지 말 것
6. category는 리스트 형식으로 작성. [[]] 사용 금지.
예시: category: [Machine-Learning]
예시: category: [Machine-Learning, Deep-Learning]