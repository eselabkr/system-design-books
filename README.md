# system-design-books

개발자 성장과 면접 대비를 위한 기술 서적 학습 노트 및 AI 활용 스터디 기록 저장소입니다.

**스터디에 참여하신다면 [스터디 운영 방식](STUDY.md)을 먼저 읽어주세요.**

## 무엇이 어디에 있나

| 경로 | 용도 |
| --- | --- |
| [`STUDY.md`](STUDY.md) | 스터디 운영 방식 · 진행 규칙 · AI 사용 규칙 |
| [`books/`](books/) | 책별 학습 노트. 한 책 = 한 디렉토리, 한 장 = 한 파일 |
| [`interview/`](interview/) | 면접 준비. 주제별 정리 · 질문 은행 · 경험 정리 · 면접 회고 |
| [`ai-log/`](ai-log/) | AI 활용 기록. 어떻게 물었고 무엇이 도움이 됐는지 |
| [`templates/`](templates/) | 노트 작성 템플릿. 새 글은 여기서 복사해서 시작 |

## 전체 구조

```
.
├── books/
│   ├── README.md                     # 책 인덱스 (진행 현황 한눈에)
│   └── <book-slug>/
│       ├── README.md                 # 책 개요 · 장별 진행 현황 · 완독 회고
│       ├── ch01-<제목>.md            # 장 노트
│       └── appendix-<제목>.md        # 부록 · 별도 정리
│
├── interview/
│   ├── README.md                     # 면접 준비 허브 · 체크리스트
│   ├── topics/                       # 주제별 지식 정리 (읽고 쌓는 곳)
│   │   ├── network/
│   │   ├── database/
│   │   ├── operating-system/
│   │   ├── data-structure-algorithm/
│   │   ├── language-framework/
│   │   └── system-design/
│   ├── questions/                    # 질문 은행 (Q&A 카드, 반복 암기용)
│   ├── experience/                   # 내 경험·프로젝트 정리 (STAR)
│   └── retrospective/                # 실제 면접 회고
│
├── ai-log/                           # AI 활용 기록
│   ├── README.md                     # 기록 인덱스 · 쌓인 패턴
│   └── YYYY-MM-DD-<주제>.md
│
├── templates/
│   ├── README.md                     # 템플릿 목록과 복사 위치
│   ├── book-readme.md
│   ├── chapter-note.md
│   ├── interview-topic.md
│   ├── interview-qa.md
│   ├── interview-retrospective.md
│   └── ai-log.md
│
├── README.md
└── STUDY.md                          # 스터디 운영 방식
```

## 세 갈래가 어떻게 이어지나

`books/`는 **입력**, `interview/`는 **출력**, `ai-log/`는 그 사이의 **과정**입니다.

책을 읽다 면접에 나올 만한 내용을 만나면, 장 노트의 *면접 예상 질문* 섹션에 적어두고
→ `interview/topics/<영역>/`의 해당 주제 문서에 내 언어로 다시 정리하고
→ 반복 암기가 필요한 것만 `interview/questions/`에 Q&A 카드로 뽑습니다.

같은 내용을 세 번 쓰는 게 아니라, **책의 맥락 → 주제별 지식 → 압축된 답변** 순으로 점점 줄여가는 흐름입니다.

그 과정에서 책의 설명만으로 막혀 AI의 도움을 받았다면, 그 경로를 `ai-log/`에 남깁니다.
결과물에는 내 문장만 들어가지만, 거기까지 어떻게 갔는지는 따로 기록으로 남는 셈입니다.
자세한 규칙은 [`STUDY.md`의 AI 사용](STUDY.md#-ai-사용)에 있습니다.

## 시작하기

새 책을 시작할 때:

```bash
BOOK=ddia   # 소문자 슬러그
mkdir -p books/$BOOK
cp templates/book-readme.md books/$BOOK/README.md
cp templates/chapter-note.md books/$BOOK/ch01-신뢰성-확장성-유지보수성.md
```

AI로 막힌 곳을 뚫었을 때:

```bash
cp templates/ai-log.md ai-log/2026-09-21-b-트리-분할.md
```

새 면접 주제를 정리할 때:

```bash
cp templates/interview-topic.md interview/topics/database/인덱스.md
```

작성 후 상위 `README.md`의 인덱스 표에 링크를 추가합니다.

## 명명 규칙

| 대상 | 규칙 | 예시 |
| --- | --- | --- |
| 책 디렉토리 | 소문자 영문 슬러그 | `ddia`, `system-design-interview` |
| 장 노트 | `ch{두 자리}-{제목}.md` | `ch03-저장소와-검색.md` |
| 부록 | `appendix-{제목}.md` | `appendix-용어정리.md` |
| 주제 정리 | `{주제}.md` (한글 가능) | `인덱스.md`, `트랜잭션-격리수준.md` |
| 면접 회고 | `YYYY-MM-DD-{회사}.md` | `2026-03-14-example-corp.md` |
| AI 활용 기록 | `YYYY-MM-DD-{주제}.md` | `2026-09-21-b-트리-분할.md` |

공백 대신 하이픈(`-`)을 씁니다.
