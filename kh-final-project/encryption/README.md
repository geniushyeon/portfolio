# 비밀번호 암호화
- 회원가입 시 사용자가 입력한 비밀번호와 `솔트`를 합친 후 `해쉬 알고리즘`을 사용해 암호화 후 저장한다.
- 로그인 시에는 사용자가 입력한 비밀번호와 DB에 저장된 솔트를 합쳐 암호화한 후, DB에 저장된 비밀번호와 비교하여 일치할 시 로그인에 성공한다.
> 처음부터 내가 맡은 부분은 아니었다. 세미 프로젝트 때 회원 파트를 맡았을 당시 비밀번호 암호화를 구현하지 못한 것이 마음에 걸려 팀원들에게 양해를 구하고 내가 구현하겠다고 이야기하였다. 구현하는 과정에서 구글링도 많이 하고, 유튜브에서 영상도 찾아보며 막연하게만 알고 있던 암호화에 한 발짝씩 다가가고 있다는 느낌을 받았다. DB에 암호화된 비밀번호가 저장되는 것을 본 첫 순간에는 정말 뿌듯했다.
## 1. 코드 보러 가기
- [암호화 코드(Utils.java)](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/java/kr/or/eutchapedia/login/controller/Utils.java)
- [service](https://github.com/geniushyeon/KH-FINAL-PROJECT/blob/main/src/main/java/kr/or/eutchapedia/login/service/MemberService.java)

## 2. 목차로 돌아가기
👉 [여기를 클릭하세요](/kh-final-project/README.md)