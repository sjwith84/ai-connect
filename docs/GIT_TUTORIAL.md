# Git 인터랙티브 튜토리얼

## 학습 목표

Git을 파일 저장소가 아니라 **프로젝트의 상태를 시간에 따라 기록하는 시스템**으로 이해한다.

## 핵심 개념

### Working Tree
현재 작업 중인 실제 파일 상태.

### Staging Area
다음 commit에 포함할 변경을 선택하는 영역.

### Commit
특정 시점의 프로젝트 상태를 하나의 기록으로 남긴다.

### Branch
기존 기록을 기준으로 독립적인 작업 흐름을 만든다.

### Remote
GitHub 같은 서버에 저장된 프로젝트의 공유본.

## 기본 흐름

```text
파일 수정
  ↓
Working Tree
  ↓ git add
Staging Area
  ↓ git commit
Commit History
  ↓ git push
Remote (GitHub)
```

## 이 프로젝트의 AI 작업 방식

ChatGPT와의 대화는 설계와 추론을 위한 공간이고, Git 저장소는 프로젝트의 영속 상태다.

새 채팅으로 이동하거나 대화 컨텍스트가 줄어들어도 다음을 읽으면 작업을 복원할 수 있도록 한다.

- `AGENTS.md`: 지속적인 작업 규칙
- `docs/DECISIONS.md`: 왜 이런 구조를 선택했는지
- `docs/CHANGELOG_AI.md`: 최근 AI 작업 내역
- 실제 코드: 현재의 최종 상태

## 인터랙티브 페이지

`index.html`에서 버튼을 눌러 Working Tree → Staging → Commit → Remote 흐름을 시각적으로 확인한다.
