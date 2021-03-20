# 별점 매기기
- 영화 상세정보 페이지에서 별점의 통계를 조회하고, 0.5점 단위로 별점을 매기거나 취소할 수 있다.

## 1. Workflow
- 비회원의 경우 로그인이 필요하다는 모달창을 출력한다.
- 로그인 후 시도할 시 Ajax를 이용하여 비동기적으로 데이터를 주고받아 view단에서 바로 확인할 수 있게끔 처리하였다.

## 2. 시연
### 2.1. 비회원
![](assets/nonmember.GIF)
- 로그인이 필요하다는 모달창을 출력한다.
### 2.2. 회원
![](assets/member.GIF)
- 0.5점 단위로 별점을 매길 수 있고, 매긴 별점을 다시 클릭하면 취소(삭제)된다.
- Ajax를 이용하여 페이지 새로고침 없이 데이터를 주고받을 수 있도록 처리하였다.
- 별점을 매긴 후 코멘트를 달 수 있으므로, 별점을 매기면 코멘트를 남길 수 있는 div가 나타난다.

## 3. 코드 보러 가기
### 3.1. 프론트엔드
- [jsp](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/webapp/WEB-INF/view/user/movie/detail/movie_detail.jsp)
- [modal](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/webapp/WEB-INF/view/user/movie/detail/modal/star_rating_non_member.jsp)
- css
  - [movie_detail_common.css(공통)](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/resources/static/css/movie/movie_detail_common.css)
  - [movie_detail.css(비회원)](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/resources/static/css/movie/movie_detail.css)
  - [movie_detail_member.css(회원)](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/resources/static/css/movie/movie_detail_member.css)
- [javascript](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/resources/static/js/movie/movie_detail_member.js)

### 3.2. 백엔드
- [controller](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/java/kr/or/eutchapedia/movie/detail/controller/StarRatingController.java)
- [domain](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/java/kr/or/eutchapedia/movie/detail/domain/StarRatingVo.java)
- [repository](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/java/kr/or/eutchapedia/movie/detail/repository/StarRatingMapper.java)
- [service](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/java/kr/or/eutchapedia/movie/detail/service/StarRatingDao.java)
- [mapper](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/resources/static/mapper/star_mapper.xml)<br/>

## 4. 목차로 돌아가기
👉 [여기를 클릭하세요](/kh-final-project/README.md)