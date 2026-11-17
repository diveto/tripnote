# TripNote 여행 플래너 PWA 패키지

이 압축 파일에는 스마트폰(iOS / Android)과 PC에서 앱처럼 설치하여 오프라인에서도 사용할 수 있는 **TripNote PWA(Progressive Web App)** 전체 파일이 포함되어 있습니다.

## 📁 포함된 파일 구조
- `index.html` : TripNote 메인 웹 애플리케이션
- `manifest.json` : 앱 이름, 테마 컬러(`#2BCBB3`), 아이콘, 독립 실행(`standalone`) 설정
- `sw.js` : 오프라인 실행 및 지도 타일 캐싱을 담당하는 Service Worker
- `icons/icon-192.png` : 표준 앱 아이콘 (192x192)
- `icons/icon-512.png` : 고해상도 앱 아이콘 (512x512)
- `icons/icon-maskable-512.png` : 안드로이드 적응형(Maskable) 아이콘 (512x512)
- `icons/apple-touch-icon.png` : iOS(아이폰/아이패드) 홈 화면 아이콘 (180x180)

---

## 🚀 무료 배포 및 스마트폰에 앱 설치하는 방법 (1분 소요)

브라우저 보안 정책상 PWA(Service Worker 및 홈 화면 설치)는 **HTTPS 웹 주소**로 접속할 때 정상 작동합니다. 아래 무료 호스팅 중 편한 곳을 이용하세요.

### 방법 1: Netlify Drop (가장 빠름 · 회원가입 후 드래그 앤 드롭)
1. 압축을 푼 폴더(`pwa_build` 또는 압축 해제 폴더)를 준비합니다.
2. [Netlify Drop](https://app.netlify.com/drop) 페이지에 접속해 폴더 전체를 화면에 끌어다 놓습니다.
3. 즉시 생성되는 `https://xxxx.netlify.app` 주소로 스마트폰에서 접속합니다.

### 방법 2: GitHub Pages (영구 무료 호스팅)
1. GitHub에 새 저장소(Repository)를 만들고 압축 파일 내 모든 파일(`index.html`, `manifest.json`, `sw.js`, `icons/` 폴더)을 업로드합니다.
2. 저장소의 **Settings → Pages → Branch(`main`)** 를 선택하고 저장하면 `https://아이디.github.io/저장소명/` 주소가 생성됩니다.

---

## 📱 기기별 앱 설치(다운로드) 방법

- **아이폰 / 아이패드 (Safari)**
  1. 배포된 `https://...` 주소로 **Safari**에서 접속합니다.
  2. 하단 **공유 버튼(⬆️)** 을 누른 뒤 **[홈 화면에 추가]** 를 선택합니다.
- **안드로이드 (Chrome / 삼성 인터넷)**
  1. 배포된 `https://...` 주소로 접속합니다.
  2. 상단 배너의 **[📲 앱 설치]** 버튼 또는 브라우저 우측 상단 메뉴(`⋮`)의 **[앱 설치 / 홈 화면에 추가]** 를 누릅니다.
- **PC (Chrome / Edge)**
  1. 주소창 우측 끝의 **설치 아이콘(⊕ / 모니터 모양)** 을 클릭하면 독립된 데스크톱 앱으로 설치됩니다.
