# AI Development Changelog

## 2026-08-09 23:39 KST

### Branch experiment: green UI + context recovery rules

**작업**
- `feature/git-branch-demo`에서 `feature/green-ui` 브랜치를 생성.
- 이 branch의 UI를 기존 파란색에서 **어두운 녹색 테마**로 변경.
- 컨텍스트 슬라이딩 이후에도 AI가 프로젝트 상태를 복원할 수 있도록 CHANGELOG/AGENTS 규칙을 강화.

**변경 파일**
- `index.html`
- `AGENTS.md`
- `docs/GIT_TUTORIAL.md`
- `docs/CHANGELOG_AI.md`

**주요 변경점**
- 전체 튜토리얼 UI의 배경, 카드, 버튼, 강조색, commit tree를 어두운 녹색 계열로 변경.
- Git branch / clone / pull / fetch / Pull Request 학습 흐름은 유지.
- `AGENTS.md`에서 작업 시작 전 최신 CHANGELOG를 읽도록 규칙화.
- 의미 있는 모든 AI 작업에 KST 날짜/시간, 작업 내용, 변경 파일, 주요 변경점, 결정 사항, 현재 상태, 다음 작업을 기록하도록 규칙화.
- CHANGELOG를 단순 이력이 아니라 **컨텍스트 슬라이딩/새 채팅 이후 AI가 작업 상태를 복원하기 위한 문서**로 정의.

**결정 사항**
- 이번 UI 변경은 기존 branch를 덮어쓰지 않고 별도의 `feature/green-ui`에서 진행한다.
- 사용자가 GitHub에서 파란색 기준 branch와 녹색 branch를 비교한 뒤 녹색 버전을 선택한다.
- 사용자의 선택 전에는 `main`에 merge하지 않는다.

**현재 상태**
- 현재 작업 branch: `feature/green-ui`
- 기준 branch: `feature/git-branch-demo`
- 녹색 UI와 문서 규칙 변경은 이 branch에 실제 commit으로 기록됨.
- `main`에는 아직 merge하지 않음.

**다음 작업**
- 사용자가 GitHub에서 `feature/green-ui`의 변경을 직접 확인.
- 녹색 UI 버전을 프로젝트 기준으로 선택하면 PR/merge 흐름을 진행.
- 이후 새 채팅 또는 컨텍스트가 줄어든 상황을 가정하고 최신 CHANGELOG + AGENTS + 실제 코드를 읽어 작업을 이어가는 복원 테스트를 수행.

---

## 2026-08-09

### Initial setup
- Git interactive tutorial project initialized.
- Added `AGENTS.md` for persistent AI development rules.
- Added `docs/GIT_TUTORIAL.md` for conceptual documentation.
- Added `docs/DECISIONS.md` for architecture decisions.
- Added `index.html`, a dependency-free interactive tutorial showing Working Tree → Staging Area → Commit → Remote.

### Branch workflow experiment
- Created the real Git branch `feature/git-branch-demo` from `main`.
- Extended `index.html` with an interactive explanation of branch creation, feature commits, remote tracking, Pull Request, merge, clone, pull, fetch, and switch.
- Updated `docs/GIT_TUTORIAL.md` with the corresponding conceptual workflow and command examples.
- The branch was intentionally kept separate from `main` so the real branch and Pull Request state could be inspected before merging.

### Verification note
- Files are being modified directly through the GitHub connection, and each file update creates a real Git commit on the selected branch.
- The tutorial's buttons simulate Git commands rather than executing local Git commands in the browser.
- The branch experiment itself is real GitHub state: `feature/git-branch-demo` is a real branch with its own commits.
