# AI Development Changelog

## 2026-08-09

### Initial setup
- Git interactive tutorial project initialized.
- Added `AGENTS.md` for persistent AI development rules.
- Added `docs/GIT_TUTORIAL.md` for conceptual documentation.
- Added `docs/DECISIONS.md` for architecture decisions.
- Added this changelog.
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
