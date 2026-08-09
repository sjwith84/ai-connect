# AI Development Rules

## Source of Truth
- GitHub repository의 현재 파일 상태를 프로젝트의 기준으로 사용한다.
- 대화 컨텍스트가 사라져도 프로젝트를 이어갈 수 있도록 중요한 지식은 문서에 기록한다.

## Before Editing
1. 관련 파일을 먼저 읽는다.
2. 최신 `docs/CHANGELOG_AI.md`를 확인해 직전 작업, 현재 branch, 변경점, 다음 작업을 파악한다.
3. `docs/DECISIONS.md`를 확인해 중요한 설계 의도를 파악한다.
4. 기존 구조와 의도를 파악한다.
5. 기존 기능을 깨뜨릴 가능성이 있는 변경은 먼저 설명하고 토론한다.

## Coding Rules
- 이 튜토리얼은 의존성 없는 순수 HTML/CSS/JavaScript를 우선한다.
- 기능을 추가할 때 기존 학습 흐름을 깨지 않는다.
- 설명 가능한 단순한 코드를 우선한다.
- 파일을 불필요하게 늘리지 않는다.

## Documentation Rules
- 중요한 설계 결정은 `docs/DECISIONS.md`에 기록한다.
- 의미 있는 모든 AI 작업은 `docs/CHANGELOG_AI.md`에 기록한다.
- CHANGELOG의 각 작업 항목에는 **한국 시간(KST) 기준 날짜와 시각**, 작업 내용, 변경 파일, 주요 변경점, 결정 사항, 현재 상태, 다음 작업을 기록한다.
- 이 로그는 단순한 이력이 아니라 컨텍스트 슬라이딩 또는 새 채팅 이후 AI가 작업 상태를 복원하기 위한 문서다.
- 사용자가 새로운 요구사항을 제시하면 기존 문서와 충돌하는지 먼저 확인한다.

## Git Rules
- 의미 있는 단위로 commit한다.
- commit 메시지는 변경 목적이 드러나게 작성한다.
- 사용자의 확인 없이 기존 작업을 되돌리거나 파괴적인 변경을 하지 않는다.
- branch를 바꿔 작업할 때 현재 branch와 변경 목적을 CHANGELOG에 명확히 기록한다.
