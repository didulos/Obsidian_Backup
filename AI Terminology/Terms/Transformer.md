---
type: term
category: [Deep-Learning, NLP, Generative-AI]
status: seed

---

## 정의

Transformer는 어텐션 메커니즘(attention mechanism)을 기반으로 순차 데이터를 병렬로 처리하는 신경망 아키텍처다. 입력 시퀀스의 모든 토큰이 동시에 처리되며, 각 토큰 간의 관계를 학습한다. 2017년 "Attention is All You Need" 논문에서 제안되었으며, 현대 대규모 언어모델(LLM)의 기반이 된다.

## 왜 중요한가

RNN/LSTM 기반 모델의 순차 처리 병목을 제거하여 대규모 데이터 학습을 가능하게 했다. ChatGPT, BERT, GPT 계열 모든 최신 모델이 Transformer 아키텍처를 사용하므로, 현대 AI 엔지니어링에서 필수 개념이다.

## 관련 개념

- 상위 개념: [[Deep-Learning]](딥러닝)

- 하위 개념: [[BERT]](버트), [[GPT]](지피티)

- 연관 개념: [[Attention]](어텐션), [[Embedding]](임베딩), [[Self-Attention]](셀프어텐션)

## 비유로 이해하기

번역가가 문장을 한 단어씩 순차적으로 번역하는 대신(RNN), 전체 문장을 동시에 보고 각 단어의 문맥상 역할을 파악한 후 번역하는 것처럼, Transformer는 모든 위치의 토큰을 한 번에 처리하면서 상호 관계를 학습한다.

## 실제 사용 예시

ChatGPT의 핵심 아키텍처로 사용되며, BERT는 양방향 Transformer를 사용해 문장 분류와 개체명 인식(NER) 같은 NLP 태스크에서 최고 성능을 달성했다.