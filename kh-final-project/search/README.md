# 영화 검색(백엔드)
- Header의 검색창에서 영화 제목, 키워드, 사용자 닉네임으로 검색 가능하다.
## 1. Workflow
- 사용자는 검색어를 입력한다.
- 결과를 출력한다.
  - 1. 상위 검색 결과: 검색어가 제목에 포함되어 있는 영화
  - 2. 영화: 상위 검색 결과 + 검색어가 DB의 키워드 테이블에 포함되어 있는 영화
  - 3. 사용자: 검색어가 닉네임에 포함되어 있는 사용자
## 2. 시연
![](assets/search.GIF)
1. 영화정보 테이블에서 `검색어가 제목에 포함된 영화`를 조회한다.
2. 영화정보 테이블과 연결된 키워드 테이블에서 `검색어가 키워드에 포함된 영화`를 조회한 후, 영화정보 테이블에서 해당 영화의 정보를 조회한다.
3. 사용자 테이블에서 `검색어가 닉네임에 포함된 사용자`를 조회한다.
4. 상위 검색 결과 탭과 영화 탭의 각 영화를 누르면 해당 영화의 상세 정보 페이지로 이동한다.
5. 사용자의 닉네임을 누르면 해당 사용자의 마이페이지로 이동한다.
- 해당 사용자의 프로필, 사용자가 담은 영화/평가한 영화 목록, 사용자가 평가한 영화의 통계 확인 가능
## 3. 코드 보러 가기
- [controller](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/java/kr/or/eutchapedia/search/controller/SearchController.java)
- domain
  - [SearchMemberVo.java](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/java/kr/or/eutchapedia/search/domain/SearchMemberVo.java)
  - [SearchMovieVo.java](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/java/kr/or/eutchapedia/search/domain/SearchMovieVo.java)
- [repository](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/java/kr/or/eutchapedia/search/repository/SearchMapper.java)
- [service](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/java/kr/or/eutchapedia/search/service/SearchDao.java)
- [mapper](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/resources/static/mapper/search_mapper.xml)

## 4. 목차로 돌아가기
👉 [여기를 클릭하세요](/kh-final-project/README.md)