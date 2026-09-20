# G3 서울플랜 · 서울 IDEA 정책실험실

HTML, CSS, JavaScript로 구성된 정적 웹사이트입니다. 별도 npm 설치나 빌드가 필요하지 않습니다.

## GitHub 업로드
1. ZIP 파일의 압축을 해제합니다.
2. 저장소의 Add file → Upload files에서 압축 해제된 내용 전체를 업로드합니다.
3. 저장소 최상위에 dist 폴더, vercel.json, README.md가 위치하도록 합니다.
4. ZIP 파일 자체를 올리는 것이 아니라 압축을 해제한 파일과 폴더를 올립니다.

## 구성
- dist/index.html: 메인 페이지
- dist/explore.html: 정책 탐색, 시민 만나기, IDEA 실습
- dist/promotion.html: 홍보 콘텐츠 프롬프트
- dist/app.js: 앱 동작 및 프롬프트
- dist/*.css, dist/*.png: 스타일과 이미지
- vercel.json: 정적 배포 설정 (출력 폴더 dist)

## 로컬 확인
프로젝트 폴더에서 `python -m http.server 8000 --directory dist` 실행 후 http://localhost:8000 에 접속하세요.

## 최신 반영사항
- 시민 페르소나와 고객여정지도 이미지 생성 요청
- 같은 Gemini 대화의 맥락을 이어가는 IDEA 프롬프트
- 아이디어 넓히기: 간결한 해외 대표사례 3개
- 실행계획 마지막에 홍보할 정책 내용과 핵심 메시지 정리
- 카드뉴스: 이미지 한 장에 6장면 (3열 × 2행)

입력 내용은 이용 중인 브라우저의 localStorage에 저장됩니다. Gemini 결과를 앱이 자동으로 수집하지 않습니다.
