---
title: "Hermes Agent와 Multi-Agent Kanban"
date: 2026-05-11
created: 2026-05-11T02:29:12
tags: [qa, hermes, multi-agent, kanban]
topic: hermes
related: []
source: claude-opus-4-6
status: archived
---

# Hermes Agent와 Multi-Agent Kanban

## Ask & Output

**Ask:**
Hermes Agent란 무엇이고, Hermes 칸반 시스템은 어떻게 동작하는가

**Output:**
Hermes Agent는 Nous Research가 만든 오픈소스 자체 개선형 AI 에이전트로, 세션 간 메모리 영속, 스킬 자동 생성, 20+ 플랫폼 게이트웨이, 7개 실행 백엔드를 지원한다. v0.13에서 도입된 Multi-Agent Kanban은 이름 있는 에이전트(Profile)들이 SQLite 기반 칸반 보드를 공유하며 Triage→Todo→Ready→Running→Done 흐름으로 작업을 자율 분담하는 시스템으로, Dispatcher가 60초마다 tick하며 워커를 배정하고 하트비트·좀비감지·환각게이트로 내결함성을 확보한다.

## Lessons Learned

- Hermes Agent는 delegate_task(동기 RPC)와 Kanban(영속 워크큐)을 용도에 따라 구분하며, Kanban의 핵심 차별점은 모든 핸드오프가 SQLite row로 남아 크래시·재시작에도 살아남는다는 것
- Hermes는 Claude Code를 워커 중 하나로 통합할 수 있어서 코딩 특화 에이전트와 범용 에이전트를 하나의 보드에서 협업시키는 구조가 가능

## Better Ask

**Before:**
Hermes Agent란 무엇이고, Hermes 칸반 시스템은 어떻게 동작하는가

**After:**
Nous Research의 Hermes Agent가 기존 AI 에이전트(Claude Code, Codex 등)와 어떤 아키텍처적 차이가 있는지, 특히 v0.13의 Multi-Agent Kanban이 delegate_task 방식 대비 어떤 내결함성·영속성 이점을 제공하는지, 실제 협업 패턴(Fan-out, Pipeline, Human-in-loop 등)별 사용 시나리오와 함께 설명해줘

---

*Related: 없음*
