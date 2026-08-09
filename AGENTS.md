# AI Development Rules

## Source of Truth
- GitHub repository의 현재 파일 상태를 프로젝트의 기준으로 사용한다.
- 대화 컨텍스트가 사라져도 프로젝트를 이어갈 수 있도록 중요한 지식은 문서에 기록한다.

## Before Editing
1. 관련 파일을 먼저 읽는다.
2. 기존 구조와 의도를 파악한다.
3. 기존 기능을 깨뜨릴 가능성이 있는 변경은 먼저 설명하고 토론한다.

## Coding Rules
- 이 튜토리얼은 의존성 없는 순수 HTML/CSS/JavaScript를 우선한다.
- 기능을 추가할 때 기존 학습 흐름을 깨지 않는다.
- 설명 가능한 단순한 코드를 우선한다.
- 파일을 불필요하게 늘리지 않는다.

## Documentation Rules
- 중요한 설계 결정은 `docs/DECISIONS.md`에 기록한다.
- AI 작업 내역은 `docs/CHANGELOG_AI.md`에 간단히 기록한다.
- 사용자가 새로운 요구사항을 제시하면 기존 문서와 충돌하는지 먼저 확인한다.

## Git Rules
- 의미 있는 단위로 commit한다.
- commit 메시지는 변경 목적이 드러나게 작성한다.
- 사용자의 확인 없이 기존 작업을 되돌리거나 파괴적인 변경을 하지 않는다.
