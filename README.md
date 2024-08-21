[![Watch the video](https://img.youtube.com/vi/UkhAaEQs3go/maxresdefault.jpg)](https://www.youtube.com/watch?v=UkhAaEQs3go)

CAREFINDER 웹 페이지 시연 영상입니다.


## PROJECT Summary

### Aug 5, 2024
- 프로젝트 리포지토리 관리 시작
- 홈 화면 구성을 위한 HTML 및 CSS 정적 페이지 작성

### Aug 6, 2024
- 홈 페이지 화면 구성 완료
- 네비게이트와 루트를 사용하여 홈에서 루트 이동 연결
- `/find` 페이지에서 병원 리스트를 카드 형태로 출력 (API 연결 전 구현)
- Find, List, Card 컴포넌트 구현
- Leftbar 각 요소에 `onClick` 이벤트 추가

### Aug 7, 2024
- 전문의 검색 API 접근 불가 확인
  - 지역 코드에 따른 요양 기호를 DB에서 가져와서 데이터 출력
  - 상위 10개의 과를 직접 입력
- 백엔드가 구성한 서버 주소로 클라이언트-서버-DB 연결 구성 시도
- GitHub 충돌 관리: Pull 대신 Merge 개념으로 상태 관리
  
### Aug 8, 2024
- API 추출 시도: 
  - 파이썬 코드로 YKIHO 엑셀 데이터 추출 및 API 요청 시도했으나
  - API 제공 질병관리청의 CORS 정책-서비스 키의 호출 제한 확인
- 회원가입 폼 작성
- `/find` 페이지에서 전문의 부분 UI 수정
- `/find` 페이지에서 시/도 선택 시 시/군/구의 선택 옵션이 변경되도록 시도(실패)

### Aug 9, 2024
- signup과 signbar가 생기면서 CSS의 충돌 수정
- 로그인 세션 방식으로 백엔드 서버와 연결
- 게시판 백엔드 서버와 연결 시도(실패)

### Aug 12, 2024
- 카카오맵 API 활용하여 병원 세부정보에 출력되도록 시도
- 게시판에서 로그인 권한 확인하도록 구현
- footer, 건강백과사전 페이지 UI 수정
- `/find`의 지역 검색 시 props 수정하여 시/도 선택 시 시/군/구의 선택 옵션이 변경되도록 구현

### Aug 13, 2024
- 뉴스 클릭 시 URL 변경 대신 상태 관리 활용하여 `/health` 페이지에서 XML 파싱 시도 성공
- 애니메이션 상태 관리 함수 작성
- 페이지 랜더링 시 파싱 속도 개선
- `find-region`, `subregion`을 코드의 키값으로 데이터 추출 가능하도록 변경
- 게시판에 필요한 로그인 세션 정보 저장 시도

### Aug 14, 2024
- 목업 데이터로 카드 리스트 및 카드 상세 출력 여부 테스트
- 카카오맵 API 테스트 및 충돌 발생: `fetch 8080`과의 충돌로 지도 로딩 문제=> ~~로 해결 
- 커뮤니티 및 게시판 UI 대규모 수정

### Aug 16, 2024
- 건강백과사전 페이지 XML 파싱 대신 JSON 사용으로 코드 간결화
- login 세션 확인 시 충돌로 인하여 실패

### Aug 18, 2024
- 로그인 후 새로고침 해야만 사용자 정보를 가져오던 세션 오류 해결
- 커뮤니티 게시판 글쓰기 및 댓글달기(로그인 확인) 구현

### Aug 19, 2024
- 조회수 기능 커뮤니티 게시판에 출력 추가 
- 게시판에 카테고리별 셀렉트박스 추가 및 검색 기능 개선
- 페이징 기능 추가: 10개 항목별로 페이지 이동
- 버튼에 `checkSession` 기능 추가
- 마이페이지 개발 진행 중(내가 찜한 병원, 내가 쓴 글 보기)

### Aug 21, 2024
- 찜하기, 글쓰기 버튼 클릭 시 세션 확인 과정 추가
- 카카오지도 마커 클릭 시 길찾기 팝업창 생성
- 마이페이지 개발 완성
