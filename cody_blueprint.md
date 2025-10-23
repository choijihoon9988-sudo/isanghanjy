# Cody Blueprint: 최재영 포트폴리오 웹사이트

## 1. 프로젝트 개요

'최재영' 개인의 포트폴리오, 경력 기술, 직무 제안을 담은 정적 웹사이트. 4개의 HTML 페이지로 구성되어 있으며, TailwindCSS를 사용해 스타일링한다.

## 2. 파일 구조

-   `index.html`: 메인 랜딩 페이지. 1년간의 성장 서사를 제시.
-   `portfolio.html`: 시각적 증거(차트, 이미지)를 통해 성과를 증명하는 페이지.
-   `resume.html`: 상세 경력 기술 및 '가치 정렬 매트릭스'를 제공하는 페이지.
-   `proposal.html`: '이상한마케팅'을 대상으로 한 구체적인 '미래 기여 제안(A2A 플라이휠)'을 담은 페이지.

## 3. 핵심 기술 스택

-   HTML
-   TailwindCSS (CDN)
-   JavaScript (DOM 조작)

## 4. 변경 기록 (Change Log)

-   **[2025-10-21]**
    -   **목표:** 4개 페이지의 내비게이션 바 통일 및 유기적 연결.
    -   **수정 파일:** `index.html`, `portfolio.html`, `resume.html`, `proposal.html`
    -   **변경 사항:**
        -   모든 페이지의 `<header>` 내 `<nav>` 요소를 "메인", "포트폴리오", "경력기술서", "미래 기여 제안" 4개의 링크가 모두 포함된 표준 내비게이션 바로 교체.
        -   `portfolio.html`, `resume.html`의 하드코딩된 활성 링크 스타일 제거.
        -   `proposal.html`의 로고 폰트 크기를 다른 페이지와 일치하도록 수정 (`text-xl` -> `text-lg`).
        -   현재 페이지 URL을 감지하여 해당 메뉴 링크에 활성 스타일을 적용하는 JavaScript 로직을 4개 파일 모두에 추가/표준화.
        -   `proposal.html`의 기존 JavaScript 로직에 있던 오타 (`| |` -> `||`) 수정 및 로직 보강.