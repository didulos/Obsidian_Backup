---
type: term
category: [NLP, Deep-Learning]
status: seed
---

## 정의

BERT(Bidirectional Encoder Representations from Transformers)는 양방향 문맥을 동시에 학습하는 사전학습 언어 모델(pre-trained language model)이다. Transformer의 인코더 구조를 기반으로 마스크된 토큰 예측(masked language modeling)과 다음 문장 예측(next sentence prediction) 작업으로 대규모 텍스트 데이터에서 학습된다. 학습된 표현(representation)을 다양한 NLP 태스크에 전이학습(transfer learning)으로 적용할 수 있다.

## 왜 중요한가

BERT는 자연어처리 분야에 전이학습 패러다임을 확립했으며, 최소한의 추가 학습(fine-tuning)만으로도 감정 분석, 개체명 인식, 의미 유사도 등 다양한 실무 태스크에서 최고 수준의 성능을 달성할 수 있다. 이로 인해 개별 태스크마다 모델을 처음부터 구축할 필요가 없어져 개발 시간과 데이터 필요량을 대폭 절감할 수 있다.

## 관련 개념

- 상위 개념: [[Transformer]](트랜스포머)

- 하위 개념: [[RoBERTa]](로버타), [[DistilBERT]](디스틸버트)

- 연관 개념: [[Transfer-Learning]](전이학습), [[Fine-tuning]](미세조정), [[Language-Model]](언어모델)

## 비유로 이해하기

BERT는 마치 수많은 책을 읽어서 언어의 규칙과 의미를 깊이 이해한 사람이 새로운 특정 작업(편지 분류, 감정 파악 등)을 빠르게 배워서 수행하는 것과 같다. 처음부터 모든 것을 학습할 필요 없이 이미 갖춘 언어 이해 능력을 바탕으로 새로운 일에 적응한다.

## 실제 사용 예시

감정 분석 태스크에서 BERT 모델을 로드한 후 영화 리뷰 데이터 500개만으로 fine-tuning하면 95% 이상의 정확도를 얻을 수 있다. 질의응답 시스템 구축 시 BERT를 인코더로 사용하여 검색된 문서 구절(passage)과 질문의 유사도를 계산하고 가장 관련 높은 답변을 반환한다.