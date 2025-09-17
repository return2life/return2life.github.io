---
# the default layout is 'page'
icon: fas fa-info-circle
order: 5
---

Git 설치하기
GitHub에 파일을 올리기 위해 아래 사이트에 접속하여 Git을 받아줍시다.
https://git-scm.com/downloads

GitHub에 Repository 만들기
깃허브 아이디가 없다면 아래 사이트에서 회원가입을 해야합니다.
https://github.com/

깃허브 접속 후 우측 상단에 프로필을 누른 후 Your profile을 눌러줍니다.

(Your repositories로 바로 들어가도 됩니다.)

Repositories를 눌러 들어가주세요.

New를 눌러 새로운 Repositories를 만듭니다.

Repository name은 원하는 이름을 입력하면 됩니다.
아래에 있는 Add a README file을 체크하시면 Repository 생성 시 README 파일이 함께 생성됩니다. 체크 후 넘어가도록 하겠습니다.

아래로 스크롤 후 생성해주시면

Repository 생성 완료입니다.

git init, add, commit
업로드할 파일을 임시로 Test라고 만들어두었습니다.
Test 폴더 안에 First.txt 파일도 함께 넣어놓았습니다.

Git을 받으면 설치되는 Git Bash를 실행시켜줍시다.
(업로드할 파일 폴더 안에서 우클릭 - Git Bash Here을 눌러 실행한다면 아래 경로로 들어가는 수고를 줄일 수 있습니다.)

실행하면 아래와 같은 화면이 나올텐데 cd [파일경로] 명령어를 통해 업로드할 폴더로 들어갑니다.




Git Bash가 처음일 경우 초기 설정을 해주어야 합니다.



git config --global user.name [GitHubName]
git config --global user.email [GitHubEmail]

이제 다시 GitHub로 갑니다.
Repository에서 Code라고 써진 곳을 클릭하여 주소를 복사합니다.
(README 추가 체크박스를 체크하지 않은 경우 안 보일 수 있습니다.)


또 다시 Git Bash로 가서 git init을 입력합니다.

그럼 해당 폴더에 .git 파일이 생성됩니다.

파일을 올려야하므로 git add . 명령어를 입력해줍시다.

여기서 뒤에 있는 .은 모든 파일을 의미합니다.
특정 파일이나 폴더를 업로드 하고 싶다면 git add First.txt와 같이 입력하면 됩니다.

그 다음 git commit -m "message" 명령어로 커밋을 합니다.

뒤에 있는 "message"는 로그입니다.
내가 어떤 작업을 했는지 기록하기 위해 작성합니다.

git push
지금까지는 파일들을 포장(커밋, commit)한 단계이고 이제부터 할 것은 이 파일들을 배송(업로드, push)할 차례입니다.

첫 push일 경우 git push -u origin master를 입력하여 push 해줍니다.

여기서 origin은 아까 복사한 경로를 붙여넣기 해주시면 됩니다.

붙여넣기 단축키: Shift + Insert

처음일 경우 GitHub Login 페이지가 뜨는데 email, password, username을 칸에 맞게 입력해주시면 됩니다.

GitHub 홈페이지에서 branch를 master로 바꾸고, (아까 push를 master로 했기 때문에)

확인했을 때 파일이 제대로 올라갔고 commit이 잘 출력되었다면 성공입니다.


파일 편집
파일을 편집했다면 위의 내용을 그대로 응용하면 됩니다.

First.txt 파일의 내용을 바꾸어보았습니다.

Git Bash에서 git add ., git commit -m "message", git push를 해줍니다.
(처음이 아니고 브런치를 바꾼 것이 아니므로 git push -u origin master를 할 필요가 없습니다.)

다시 GitHub 홈페이지에서 확인해보면

commit한 내용 그대로 velog Test v0.2로 바뀐 것을 볼 수 있습니다.

당연하게도 내용 또한 바뀌었습니다.
velog Test v0.2 부분을 누르면

어느 부분이 바뀌었는지 확인할 수 있습니다.

