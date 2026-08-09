# AI Development Changelog

## 2026-08-09 23:39 KST

### Branch experiment: green UI + context recovery rules

**작업**
- `feature/git-branch-demo`에서 `feature/green-ui` 브랜치를 새로 생성.
- 기존 파란색 UI를 기준으로, 이 브랜치에서 어두운 녹색 UI로 변경할 예정.
- 컨텍스트 슬라이딩 이후에도 AI가 프로젝트 상태를 복원할 수 있도록 CHANGELOG 규칙을 강화.

**변경 파일**
- `AGENTS.md`
- `docs/CHANGELOG_AI.md`
- 다음 단계: `index.html`, `docs/GIT_TUTORIAL.md`, 필요 시 `docs/DECISIONS.md`

**변경점**
- `AGENTS.md`에 작업 시작 전 최신 CHANGELOG를 읽도록 규칙 추가.
- 모든 의미 있는 AI 작업에 KST 날짜/시간, 작업 내용, 변경 파일, 주요 변경점, 결정 사항, 현재 상태, 다음 작업을 기록하도록 규칙 추가.
- CHANGELOG를 단순 기록이 아니라 **컨텍스트 슬라이딩/새 채팅 이후 AI의 작업 상태 복원 문서**로 정의.

**현재 상태**
- 현재 작업 branch: `feature/green-ui`
- 기존 기준 branch: `feature/git-branch-demo`
- `main`에는 아직 이번 녹색 UI 변경을 merge하지 않음.
- 이번 단계에서는 branch를 실제로 분리하고 AI 복원 규칙을 먼저 적용함.

**다음 작업**
- `index.html`의 전체 UI 테마를 파란색에서 어두운 녹색으로 변경.
- 관련 Git 튜토리얼 Markdown에 branch 실험의 의도를 기록.
- 변경 내용을 이 branch에 commit.
- 사용자가 GitHub에서 두 branch의 차이를 확인한 뒤 녹색 branch를 선택할지 결정.

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
- The branch is intentionally kept separate from `main` so the real branch and Pull Request state can be inspected before merging.

### Verification note
- Files are being modified directly through the GitHub connection, and each file update creates a real Git commit on the selected branch.
- The tutorial's buttons simulate Git commands rather than executing local Git commands in the browser.
- The branch experiment itself is real GitHub state: `feature/git-branch-demo` is a real branch with its own commits.
