# S2.A1.L1 — Architecture (아키텍처 설계)

## 기술 스택
```
Frontend: Vanilla HTML5 + CSS3 (Custom Properties) + ES6 JS
CDN: Google Fonts (Inter)
API: Gemini API (chatbot.html)
Hosting: GitHub Pages (static)
```

## CSS 설계 원칙

### CSS Custom Properties (Root Variables)
```css
:root {
  --bg:      #050c1a;   /* 페이지 배경 */
  --bg2:     #0b1a30;   /* 섹션 배경 */
  --bg3:     #0f2240;   /* 서브 섹션 */
  --card:    #1e5ab5;   /* 카드 시작 */
  --card2:   #2469c8;   /* 카드 끝 */
  --border:  rgba(0,212,255,0.6);
  --text:    #f0f5fb;
  --cyan:    #00d4ff;
  --purple:  #7c3aed;
  --green:   #10b981;
}
```

### 3-Level Color Hierarchy
```
L1: #050c1a (페이지 배경)
L2: #0b1a30 (섹션 배경)
L3: #1e5ab5 → #2469c8 (카드 그라디언트)
```

## 파일 구조
```
/
├── index.html        — 메인 (Hero + Stats + Features + CTA)
├── architecture.html — 아키텍처 (SVG 다이어그램 + 탭)
├── manual.html       — 매뉴얼 (사이드바 + 아코디언)
├── chatbot.html      — 챗봇 (사이드바 + 채팅 + 모달)
├── dashboard.html    — 대시보드 (KPI 카드 + 차트)
└── agents.html       — 에이전트 (카드 그리드 + 검색)
```

## 브랜드 식별 요소
- **Rainbow Top Bar**: `border-image: linear-gradient(90deg, #00d4ff, #7c3aed, #10b981, #f59e0b) 1`
- **Cyan Glow**: `box-shadow: 0 4px 25px rgba(0,212,255,0.2)`
- **Blue Cards**: `linear-gradient(135deg, #1e5ab5, #2469c8)`
