# Remove_bg — 배경제거

> 배경은 빼고, 당신만 남깁니다.

AI 기반 배경 제거 웹앱. 서버 전송 없이 브라우저에서 완전히 로컬로 처리됩니다.

![Remove_bg](https://img.shields.io/badge/Remove__bg-배경제거-2dd4bf?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-brightgreen?style=flat-square)

---

## 주요 기능

- **AI 자동 배경 제거** — `@imgly/background-removal` 라이브러리 기반 (WASM + ONNX 모델)
- **완전 로컬 처리** — 이미지가 서버로 전송되지 않음, 개인정보 보호
- **PNG / JPG 저장** — PNG(투명 배경) 또는 JPG(배경색 선택) 형식으로 저장
- **해상도 선택** — 고해상도(원본) / 저해상도(50% 축소) 선택 저장
- **before / after 비교 슬라이더** — 원본과 결과물을 드래그로 비교
- **엣지 후처리** — 배경제거 후 가장자리 컬러 프링징 제거 + 알파 스무딩
- **반응형 디자인** — 모바일 · 태블릿 · PC 대응

---

## 사용법

별도 설치나 빌드 없이 `index.html` 파일 하나로 동작합니다.

```
index.html 파일을 브라우저에서 바로 열거나
GitHub Pages, Netlify 등에 배포하세요.
```

### 캘리그라피 이미지 설정

`index.html`과 같은 폴더에 `calli.png` 파일을 넣으면 첫 화면 하단에 표시됩니다.

- 배경이 제거된 PNG 파일 (투명 배경 + 검정 글씨)
- CSS `filter: invert(1)`로 자동 흰색 반전 처리

---

## 기술 스택

| 항목 | 내용 |
|------|------|
| 런타임 | 순수 HTML + CSS + JavaScript (빌드 도구 없음) |
| AI 모델 | [@imgly/background-removal](https://github.com/imgly/background-removal-js) v1.7.0 |
| 폰트 | Inter (Google Fonts) |
| 아이콘 | Lucide Icons (인라인 SVG) |
| 배포 | GitHub Pages |

---

## 파일 구조

```
/
├── index.html   # 앱 전체 (HTML + CSS + JS 단일 파일)
└── calli.png    # 캘리그라피 이미지 (선택)
```

---

## 배포

GitHub Pages를 사용하는 경우:  
저장소 Settings → Pages → Branch: `main` / `/(root)` 로 설정하면 바로 배포됩니다.

---

## 크레딧

&copy; Produced by You Seungoh.  
[yso21@naver.com](mailto:yso21@naver.com) | [youtube.com/@pianocanvas](https://youtube.com/@pianocanvas) | Healing Cafe Music
