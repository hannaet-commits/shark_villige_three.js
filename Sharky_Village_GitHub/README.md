# Sharky Village · 3D 상어 마을

Three.js 0.170.0으로 만든 바닷속 마을과 영어 퀴즈입니다.

## GitHub에 올리기
1. ZIP을 압축 해제합니다.
2. GitHub 저장소에서 Add file → Upload files를 선택합니다.
3. 압축 해제한 파일을 모두 올리고 Commit changes를 누릅니다.
   index.html이 저장소 첫 화면(루트)에 있어야 합니다. ZIP 자체를 올리는 것이 아닙니다.
4. 웹사이트로 실행하려면 Settings → Pages에서 Source를 Deploy from a branch로 선택합니다.
5. Branch: main, 폴더: /(root)를 선택하고 Save를 누릅니다.
6. 배포 완료 후 Pages에 표시되는 사이트 주소로 접속합니다.
   계정과 저장소 공개 범위에 따라 Pages 사용 가능 여부가 다를 수 있습니다.

## 내 컴퓨터에서 실행
JavaScript 모듈을 사용하므로 index.html을 더블클릭하는 방식 대신 웹 서버로 실행하세요.
- Cursor 또는 VS Code의 Live Server 확장에서 index.html을 엽니다.
- Python이 설치되어 있다면 이 폴더에서 `python -m http.server 8000`을 실행하고
  브라우저에서 http://localhost:8000 을 엽니다.

## 조작
- 드래그: 시점 회전 / 마우스 휠: 확대 및 축소
- 아래 장소 버튼: 산호 광장, 조개집, 상어 학교, 보물 정원 이동
- 마을 산책하기: 자동 회전
- 상어 클릭 또는 영어 놀이 버튼: 영어 퀴즈 5문항
- 영어 문장 듣기: 브라우저의 영어 음성 합성 사용
- 바다별은 현재 페이지 세션에만 유지됩니다.

## 파일
- index.html: 화면 구성
- style.css: 디자인 (Google Fonts 사용, 연결 실패 시 기본 글꼴)
- app.js: 3D 마을, 애니메이션, 퀴즈
- three.module.js: Three.js 라이브러리 (포함되어 있어 CDN 로딩 불필요)
- THREE-LICENSE.txt: Three.js MIT 라이선스
- .nojekyll: 정적 파일 배포용

## 실행 환경과 검증
WebGL 2를 지원하는 브라우저 및 그래픽 환경이 필요합니다.
JavaScript 문법 검사와 ZIP 무결성을 확인했습니다.
제작 시 확인용 브라우저의 WebGL 제한으로 실제 3D 렌더링 및 클릭 동작 검증은 완료하지 못했습니다.
