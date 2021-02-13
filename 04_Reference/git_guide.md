## Git Guide

- [git과 atom 연동하기](https://m.blog.naver.com/wlgh325/221443819508)
- [git과 vscode 연동하기](https://technote.kr/352)

## 필수 명령어
- git status
    - 현재 git 상태 확인

- git branch
    + 현재 브랜치 확인
        - administrator branch는 master로 통일

    + git branch 브랜치명
        - git branch 생성

    + git branch -d 브랜치명
        - 브랜치명 branch 삭제

- git checkout 브랜치명
    + 본인에게 할당된 브랜치로 전환
        - 일반적으로 master 내 본인 브랜치를 사용하면 됨
        - i.g. git checkout choi or git checkout kim

- git diff 파일명
    + 변동된 내용 확인
    + i.g. git diff a.py

- git add 파일명
    + 변경 또는 생성된 파일 또는 폴더 반영
    + i.g. git add a.py

- git commit
    + commit message 기록 및 저장
    + commit

- git merge origin/브랜치명
    + 변경 또는 추가 된 내용 병합
    + i.g. git merge origin/choi

- git push origin 브랜치명
    + repository에 반영
    

### 가장 기초적인 git process
1. git, vscode, vim, atom 등을 통해 github or gitlab과 연동된 local 폴더로 진입
2. git status를 통해 현재 repo 상태 확인
    + (필요 시 git branch 확인 후 원하는 branch로 진입)
3. git fetch -> git pull origin master를 통해 최신 데이터를 local로 가져옴
4. 폴더 및 파일 생성, 변동
5. git status
    + 변동된 내용이 터미널에 출력됨
    + 내용을 자세히 보려면 git diff 파일명
6. git commit 후 엔터
    + commit 메시지 작성
    + 간략, 명확할 수록 좋음
7. git commit message 작성 후 저장
    + git commit -m "commit message" 라고 간단하게 작성도 가능
8. git status 확인
    + commit 이 제대로 되었을 시 특별한 메시지가 따로 뜨지 않음
9. git push origin 브랜치명
    + i.g. git push origin choi
10. (master 하위 브랜치 이용시) push 후 github pull request 
<img src="https://www.secmem.org/assets/images/git_pr/github_pullrequest.png">
    + pull request 요청
    + master brach 관리자가 해당 내용을 repo에 반영 

