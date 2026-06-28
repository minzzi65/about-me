# 🦫 채민지 — About Me

## 완료 작업 목록

- 바닐라 HTML, CSS로 자기소개용 정적 웹 페이지 구현 (`index.html` / `style.css` 분리)
- 능소화 색상을 배경으로 한 명함 카드 컨셉 UI 구현 (프로필, 관심 분야, 기술 스택, 링크 섹션 포함)
- Python, C, PyTorch, TensorFlow 기술 스택을 devicons 아이콘 카드로 시각화
- GitHub, 네이버 블로그 외부 링크 버튼 구현
- 반응형 레이아웃 및 마이크로 애니메이션 적용

### 동작 화면

![about-me 페이지 실행 화면](./preview.png)

## 설계 과정

능소화 색상을 CSS 변수(`--campsis-*`)로 토큰화하여 전체 색상 시스템을 설계했습니다. 관심 분야(딥러닝, 임베디드 AI)와 기술 스택은 각각 독립 카드로 분리해 가독성을 높였고, HTML과 CSS 파일을 분리하여 구조와 스타일의 역할을 명확히 구분했습니다.

## AI를 활용한 부분

- 능소화 색상에 어울리는 색상 코드 추천 및 CSS Flexbox/Grid 레이아웃 코드 작성에 활용
- 딥러닝·임베디드 분야 소개 문구를 전문적으로 다듬는 데 활용
- devicons CDN 연동 및 `color-mix()` 활용법을 AI에게 질문하며 기술 스택 섹션 구현

## 새로 알게 된 것

**CSS Custom Properties** — 색상을 변수로 토큰화하면 값 하나만 바꿔도 전체 스타일이 일괄 변경된다는 것을 직접 경험했습니다.

**CSS Grid** — `grid-template-columns: 1fr 1fr`로 2열 레이아웃을 만들고 미디어 쿼리로 1열 전환하는 반응형 패턴을 익혔습니다. 2차원 배치는 Flexbox보다 Grid가 더 적합하다는 점도 이해했습니다.

**CDN 활용** — `devicons` 라이브러리를 `<link>` 한 줄로 불러와 `<i class="devicon-python-plain">` 형태로 아이콘을 바로 쓸 수 있다는 게 편리했습니다.