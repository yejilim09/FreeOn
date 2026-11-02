# FREEON

배리어프리 통합 플랫폼 시제품 (정적 사이트 · GitHub Pages)

## 폴더 구성
- `index.html` : 사이트 본체
- `facilities.json` : 전국 배리어프리 시설 데이터
- `events.json` : 행사 데이터 (행사 시트 기준, 행사 장소는 지도에도 표시)
- `images/` : 행사 포스터·상품 사진

## 카카오 지도 키
`index.html`에서 `여기에_키_붙여넣기`를 검색해 카카오 **JavaScript 키**로 바꿔 주세요.
카카오 개발자 콘솔 > 플랫폼 > Web에 배포 주소(`https://아이디.github.io`)도 등록해야 지도가 보여요.

## images 폴더 파일 이름
- `event-poster-1.jpg` : 서울배리어프리영화제
- `event-poster-2.jpg` : 김현철의 유쾌한 오케스트라
- `event-poster-3.jpg` : 앤ANNE: 배리어프리
- `keyring.jpg` : NFC 오디오북 키링
- `boardgame.jpg` : 손끝의 달인: 암흑 속의 결투
- `second-game.jpg` : 우주 메리미

## 참고
커뮤니티 글·좋아요·댓글과 장바구니는 지금 각자의 브라우저(localStorage)에만 저장돼요.
다른 사람과 글을 공유하려면 데이터베이스 연결이 필요합니다.
