    1. https://git-scm.com 에 접속하여 Git-2.27.0-64-bit을 다운로드하여 설치

    2. 설치시 두 번째 대화상자의 선택 옵션에서 Use Git from the windows Command Orompt를 선택하여 설치할 것.

    3. 설치가 끝나면 git bash를 시작메뉴에서 찾아 실행

    4. 기본 버전 명령 : git --version, 도움말 확인 명령 : git --help

    5. github.com에 접속하여 로그인

    6. git bash에서 프로젝트 폴더를 만듦
        ex1) cd d:\; 엔터
        ex2) mkdir jyj
        ex3) cd jyj
        ex4) mkdir test-code
        ex5) ls -al

    7. git bash에서 ssh-keygen 명령으로 암호키를 생성

    8. 내컴퓨터에서 생성된 키젠이 있는 디렉토리로 이동해서 id_rsa.pub파일을 찾아 열고 그 안의 내용을 복사하기 한다.

    9. 로그인 된 github에서 가장 오른쪽의 메뉴의 Setting을 선택하고, 가장 왼쪽 메뉴의 여덟번째의 SSH and GPG를 선택

    10. SSH 항목의 [new SSH key]버튼을 눌러 나오는 창에
    title : ssh key
    key : 복사하기한 id_rsa.pub파일의 내용을 붙여넣기하여 키를 등록

    11. git bash에서 사용자를 등록
        git config --global user.name "사용자아이디"
        git config --global user.email "사용자이메일주소"

    12. git bash에서 해당 프로젝트 디렉토리를 초기화
        git init

    13. 프로젝트 개발코드 입력하고 저장
        README.md 작성

    14. git bash에서 관리목록으로 추가
        git add 파일명 또는 git add .

    15. git의 상태보기(빨간색은 아직 add하지 않은 것, 초록색은 add한 내용)
        git status

    16. 작업한 내용의 메시지를 기록
        git commit -m "커밋할메시지(작업내용)"

    17. 원격저장소 지정
        git remote add origin 해당레포시토리주소
                                (https://github.com.dudwn7504/test-code)
    
    18. 원격저장소에 업로드
        git push -u origin master

    19. 해당하는 아이디나 이메일, 패스워드를 물어볼 경우 입력하면 업로드 성공!