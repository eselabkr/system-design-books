# AI 활용 기록

책을 읽다 막힌 곳을 AI로 뚫었을 때, **어떻게 물었고 무엇이 도움이 됐는지**를 남기는 곳입니다.

정리된 지식은 [`books/`](../books/)와 [`interview/topics/`](../interview/topics/)에 있습니다.
여기 남기는 것은 지식이 아니라 **그 지식에 도달한 과정**입니다.

규칙은 [`STUDY.md`의 AI 사용](../STUDY.md#-ai-사용)을 참고하세요.

## 무엇을 남기나

- 책의 설명으로는 이해가 안 됐던 지점과, 결국 이해하게 된 경로
- 효과가 있었던 질문 방식 — 왜 그 질문이 통했는지까지
- **AI가 틀리게 답한 사례** — 가장 값어치 있는 기록입니다. 어떻게 틀렸고 어떻게 알아챘는지 남겨주세요
- 검증 없이 믿었다가 나중에 뒤집힌 내용

## 무엇을 남기지 않나

- AI가 생성한 설명 자체를 그대로 옮겨 적는 것
- "편했다" 수준의 감상

## 남기는 법

한두 줄짜리 도움말이면 장 노트의 *AI 활용 기록* 섹션으로 충분합니다.
따로 파고든 주제만 여기에 문서로 남깁니다.

```bash
cp templates/ai-log.md ai-log/<이름>/2026-09-21-b-트리-분할.md
```

위치 : `ai-log/<이름>/` · 파일명 : `YYYY-MM-DD-{주제}.md`

## 기록

| 날짜 | 작성자 | 주제 | 관련 | 분류 | 문서 |
| --- | --- | --- | --- | --- | --- |
| 2026-10-07 | yeol | 데이터가 아주 많을 때 왜 NoSQL이 유리한가 | [system-design-interview ch.1](../books/system-design-interview/yeol/ch01-사용자-수에-따른-규모-확장성.md) | 🟢 이해에 도움 | [문서](yeol/2026-10-07-nosql-수평-확장.md) |
| 2026-10-13 | yeol | 규모 추정 "더 알아볼 것" (디스크 지연, GPU 병목, 압축, 고가용성, QPS) | [system-design-interview ch.2](../books/system-design-interview/yeol/ch02-개략적인-규모-추정.md) | 🟢 이해에 도움 | [문서](yeol/2026-10-13-규모-추정-더-알아볼-것.md) |
| 2026-10-13 | yeol | AI(바이브 코딩, 에이전트)가 시스템 설계에 미친 영향 | [system-design-interview ch.3](../books/system-design-interview/yeol/ch03-시스템-설계-면접-공략법.md) | 🟡 검증 필요 | [문서](yeol/2026-10-13-ai-시대-시스템-설계-변화.md) |
| 2026-10-13 | yeol | 시스템 설계 핵심 컴포넌트의 세부 기능과 동작 순서 | [system-design-interview ch.3](../books/system-design-interview/yeol/ch03-시스템-설계-면접-공략법.md) | 🟡 검증 필요 | [문서](yeol/2026-10-13-시스템-설계-컴포넌트-동작-순서.md) |
| 2026-10-13 | rani | 2·3장 개념 정리 (가용성, 지연시간, 메시지 큐, QPS 계산 등) | [system-design-interview ch.2·3](<../books/system-design-interview/rani/ch02-개략적인-규모-추정+ch03-효과적-면접을-위한-4단계-접근법.md>) | 🟢 이해에 도움 | [문서](rani/2026-10-13-ch02-ch03-개념-정리.md) |
| 2026-10-19 | rani | 4장 개념 정리 (HTTP·TLS, 429, API 게이트웨이, 이동 윈도 카운터 등) | [system-design-interview ch.4](../books/system-design-interview/rani/ch04-처리율-제한-장치의-설계.md) | 🟢 이해에 도움 | [문서](rani/2026-10-19-ch04-처리율-제한-개념-정리.md) |
| 2026-10-19 | rani | 5장 개념 정리 (해시 링, 가상 노드, 파티션, 복제 등) | [system-design-interview ch.5](../books/system-design-interview/rani/ch05-안정-해시.md) | 🟢 이해에 도움 | [문서](rani/2026-10-19-ch05-안정-해시-개념-정리.md) |

> 분류: 🟢 이해에 도움 · 🔴 AI가 틀림 · 🟡 검증 필요

## 쌓이면 볼 것

<!-- 기록이 어느 정도 모이면 여기에 패턴을 정리합니다. -->

### 잘 통한 질문 방식

-

### AI가 자주 틀리는 영역

-
