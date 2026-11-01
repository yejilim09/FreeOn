# FREEON — 배리어프리 통합 웹앱 시제품

## 실행
1. `index.html`을 브라우저에서 열면 지도 API 키 없이도 화면과 기본 메뉴를 확인할 수 있습니다.
2. 실제 카카오 지도를 연결하려면 카카오디벨로퍼스에서 앱을 만들고 카카오맵을 활성화하세요.
3. 앱의 **JavaScript 키**를 복사해 `index.html`의 `KAKAO_JS_KEY` 값에 넣습니다.
4. 카카오디벨로퍼스의 JavaScript SDK 도메인에 테스트 주소와 배포 주소를 등록합니다.
5. GitHub 저장소에 `index.html`을 올리고 Settings → Pages에서 배포합니다.

공식 문서:
- https://developers.kakao.com/docs/ko/kakaomap/common
- https://developers.kakao.com/docs/ko/kakaomap/web
- https://docs.github.com/pages

## 현재 구현된 시제품 기능
- PC·모바일 반응형 화면
- 홈 / 시설 지도 / 행사 / 스토어 / 커뮤니티 메뉴 전환
- 시설 목록 검색 및 접근성 필터
- 카카오맵 JavaScript SDK 연결 자리와 마커 코드
- 행사 검색 및 편의 유형 필터
- 상품 카테고리 필터
- 커뮤니티 글쓰기 화면 (현재 브라우저 메모리에서만 임시 반영)
- 글자 크기 조절, 키보드 포커스 표시, 스킵 링크, 기본 스크린리더 레이블

## 주의
시설·행사·상품은 모두 시제품용 예시 데이터입니다. 실제 정보나 실제 판매 상품이 아닙니다.
리뷰, 계정, 게시글 공유, 장바구니, 결제는 아직 서버/데이터베이스에 연결되지 않았습니다.
카카오 JavaScript 키는 웹에 노출되는 브라우저용 키입니다. REST API 키나 관리자 키 등 비밀 키를 HTML에 넣지 마세요.

## 확장할 때 권장하는 파일 구조
처음에는 초보자가 수정하기 쉽도록 단일 `index.html`로 시작합니다. 기능이 안정되면 다음 구조로 분리합니다.

```text
FREEON/
├── index.html
├── assets/
│   ├── images/
│   └── icons/
├── css/
│   ├── style.css
│   └── responsive.css
├── js/
│   ├── app.js
│   ├── map.js
│   ├── events.js
│   ├── store.js
│   └── community.js
└── README.md
```
