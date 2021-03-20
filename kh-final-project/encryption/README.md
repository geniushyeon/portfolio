# 비밀번호 암호화
- 회원가입 시 사용자가 입력한 비밀번호와 `솔트`를 합친 후 `해쉬 알고리즘`을 사용해 암호화 후 저장한다.
- 로그인 시에는 사용자가 입력한 비밀번호와 DB에 저장된 솔트를 합쳐 암호화한 후, DB에 저장된 비밀번호와 비교하여 일치할 시 로그인에 성공한다.
## 1. 코드 보러 가기
- [암호화 코드(Utils.java)](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/java/kr/or/eutchapedia/login/controller/Utils.java)
- [service](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/java/kr/or/eutchapedia/login/service/MemberService.java)

## 2. 목차로 돌아가기
👉 [여기를 클릭하세요](/kh-final-project/README.md)