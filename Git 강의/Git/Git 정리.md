# 1. 정의

Q. Git이 뭐야??

A. **분산 버전 관리** 시스템이야!!!

\- Git 은 변경 사항만을 저장한다. -> 용량이 적어지고 프로그램이 가벼워진다.

\- Git 과 GitHub는 다르다.



# 2. Git & VSCode설치

## 1) Git 설치

![git 설치_1](Git%20%EC%A0%95%EB%A6%AC.assets/git%20%EC%84%A4%EC%B9%98_1.PNG)



## 2) VSCode 설치

![vscode 설치](Git%20%EC%A0%95%EB%A6%AC.assets/vscode%20%EC%84%A4%EC%B9%98.PNG)



# 3. Git 사용

CLI(Command-Line-Interface)를 통해서 사용

cf. GUI

## 1) 간단한 Unix/Linux 명령어

-ls : 형재 위치의 폴더, 파일 목록보기

-cd \<path>: 현재 위치 이동하기

-cd .. : 상위 폴더로 이동

-mkdir \<name> : 폴더 생성하기

-touch \<name> : 파일 생성하기

-rm : 파일 한 개를 지우는 명령어

-rm -r : 폴더를 지우는 명령어



## 2) Repository

\- 특정 디렉토리를 버전 관리하는 저장소

- git init 명령어로 **로컬 저장소**를 생성한다.



# 4. RacingRound 프로젝트 실습

## 1) Commit 의 3가지 영역



-특정 버전으로 남긴다 = "커밋(Commit)" 한다.

1. **working Directory** : 작업하고 있는 실제 디렉토리(.git 이 있는 디렉토리)
2. **Staging Area** : 커밋으로 남기고 싶은, 특정 버전으로 관리하고 싶은 파일이 있는곳
3. **Repository** : 커밋들이 저장되는곳



-Working Directory에 있는 untracked 상태의 파일을 **git add** 명령어를 통해 

 tracked 상태로 바꿔 Staging Area에 올린다.

-**git commit** 명령어를 통해 하나의 버전으로 남아 Repository에 저장한다. (commit 01)

-commit 01 된 파일은 modified 파일

-modified 파일을 git add -> git commit 을 통해 새로운 버전인 commit 02 생성

-위의 과정을 통해 버전을 관리한다.



## 2) git 명령어

-git init

-git add : 버전관리를 하고 싶은 파일들만 add를 해준다.

-git add . : 추척되지 않은 모든파일과 수정된 파일을 모두 Staging Area에 올림

-git status

-git commit -m "commit_message" : 커밋과 커밋 메세지를 등록(커밋 메세지는 최대한 자세히!!!)

-git config --global user.name

-git log : git의 commit history를 본다.

-git diff : 주소를 통해 이전 commit들의 변경사항을 비교한다.



## 3) github 연동

-git remote add origin {원격 저장소의 주소} 

![git 원격 저장소 주소](Images/Git%20%EC%A0%95%EB%A6%AC/git%20%EC%9B%90%EA%B2%A9%20%EC%A0%80%EC%9E%A5%EC%86%8C%20%EC%A3%BC%EC%86%8C.png)

-git push -u origin master : master 브랜치에 올린다.

-git push origin master : 위에랑 차이가 뭔지 질문

-git clone {원격 저장소} : 원격 repo를 로컬로 복사한다.



