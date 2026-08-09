# AI Connect — Git Interactive Tutorial

ChatGPT와 GitHub를 함께 사용하면서 **대화의 컨텍스트와 프로젝트의 영속 상태를 분리**하기 위한 작은 실험 프로젝트입니다.

## 목적

- `index.html`: 브라우저에서 Git의 기본 흐름을 인터랙티브하게 학습
- `AGENTS.md`: AI가 프로젝트를 수정할 때 지켜야 할 지속적인 규칙
- `docs/GIT_TUTORIAL.md`: 튜토리얼의 개념과 사용법
- `docs/DECISIONS.md`: 중요한 설계 결정을 기록
- `docs/CHANGELOG_AI.md`: AI와 함께 작업한 변경 내역 기록

## 핵심 원칙

1. Git 저장소의 현재 파일 상태를 프로젝트의 기준(Source of Truth)으로 삼는다.
2. 대화 내용에만 의존하지 않고 중요한 설계 의도는 Markdown 문서에 기록한다.
3. 기존 구조를 읽고 이해한 뒤 수정한다.
4. 큰 구조 변경은 먼저 토론하고, 합의된 내용을 `DECISIONS.md`에 남긴다.
5. 작업이 끝나면 변경 내용을 설명하고 Git 기록으로 남긴다.

## 시작

`index.html`을 브라우저에서 열어 Git의 기본 흐름을 체험할 수 있습니다.
