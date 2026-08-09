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
특정 commit을 가리키는 이름표이며, 독립적인 작업 흐름을 만들 수 있다.

### Remote
GitHub 같은 서버에 저장된 프로젝트의 원격 저장소다. `origin`은 흔히 이 원격 저장소를 가리키는 이름으로 사용한다.

### Pull Request
한 branch의 변경을 다른 branch에 합치기 전에 검토하고 논의하기 위한 GitHub의 협업 단위다.

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

## Branch 협업 흐름

```text
main:    A ── B ───────────── M
              \             /
feature:       C ── D ──────

C/D를 만든 뒤 push
        ↓
Pull Request: feature → main
        ↓
Merge
        ↓
main에 M으로 통합
```

## 다른 컴퓨터에서 받기

### 처음 프로젝트를 받는 경우

```bash
git clone <repository-url>
cd ai-connect
```

`clone`은 원격 저장소의 파일과 Git 이력을 새 로컬 저장소로 가져오는 작업이다.

### 이미 clone한 프로젝트를 최신화하는 경우

```bash
git switch main
git pull
```

`pull`은 원격의 최신 변경을 가져와 현재 branch에 통합한다. 따라서 다른 컴퓨터에서도 GitHub에 반영된 프로젝트 상태를 따라갈 수 있다.

### 원격 feature branch를 확인하는 경우

```bash
git fetch origin
git switch feature/git-branch-demo
```

`fetch`는 원격의 변경 정보를 가져오고, `switch`는 작업할 branch를 선택한다.

## 이 프로젝트의 AI 작업 방식

ChatGPT와의 대화는 설계와 추론을 위한 공간이고, Git 저장소는 프로젝트의 영속 상태다.

새 채팅으로 이동하거나 대화 컨텍스트가 줄어들어도 다음을 읽으면 작업을 복원할 수 있도록 한다.

- `AGENTS.md`: 지속적인 작업 규칙
- `docs/DECISIONS.md`: 왜 이런 구조를 선택했는지
- `docs/CHANGELOG_AI.md`: 최근 AI 작업 내역
- 실제 코드: 현재의 최종 상태

## 인터랙티브 페이지

`index.html`에서 다음 흐름을 버튼으로 확인한다.

1. Working Tree → Staging → Commit → Remote
2. main → feature branch → feature commits → push
3. Pull Request → merge
4. 다른 작업공간에서 clone / pull / fetch / switch

페이지의 버튼은 **실제 Git 명령을 실행하는 것이 아니라 개념을 시각화**한다. 실제 branch와 commit은 이 튜토리얼 repository 자체에서 확인할 수 있다.
