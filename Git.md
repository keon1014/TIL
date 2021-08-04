# Git & GitHub

> 컴퓨터 파일의 변경 사항을 추적하고 여러 명의 사용자들 간에 해당 파일들의 작업(협업)을 조율하기 위한 분산 버전 관리 시스템(리누스 토발즈(Linus Torvalds) 최초 개발)
>
> SCM(Source Code Management, 코드 관리도구) = VCS(Version Control System, 버전 관리 도구)



#### 버전관리란? 

- 파일을 버전별로 저장하여 관리

  (일반적으로는 파일을 계속 다른 이름으로 저장(복사해서 제목수정)하니 파일이 무한정으로 늘어남)

- 동일한 정보에 대해 여러버전을 관리하는 것.

- 과거버전으로 돌아가 사용할 수 있고, 변경 history를 알 수 있음. 

  

#### Git 설치 후 Git Bash 실행



## CLI 기본명령어 

CLI : Command Line Interface

GUI  : 윈도우 환경과는 다른 인터페이스를 지닌다.



- **ls**(list) : 현재 디렉토리(폴더) 목록

- **pwd**(print working directory) : 현재 디렉토리(폴더) 위치, 디렉토리 경로, 작업중인 디렉토리 위치

- **mkdir**(make directory) : 디렉토리 만들기

- **cd**(change directory) : 디렉토리이동
  
  - ```cd .. ``` : 상위 디렉토리 이동
  - ```cd. ```     : 현재 디렉토리 이동
  - ```cd ~ ```    : 홈 디렉토리 이동 이동
  - ```cd / ```     : 루트/최상위 디렉토리로 이동
  - ```cd  ```       : 홈 디렉토리(기본값)로 이동
  
- **touch** :  새로운 파일 만들기

  





## Git 기본 명령어  

==저장소 만들기==
git init

==작업 후 버전기록==
git add .
git commit -m '커밋메시지'

==상태 보기==
git status
git log

==원격저장소==
git remote add origin <url>
git push origin master



```bash
$ git status
On branch master
# 트래킹되고 있지 않은 파일들 (Working directory)
Untracked files:
# Staging area에 포함시키기 위해서는 git add를 해.
# Staging area -> 커밋 대상 파일들 모아놓는 공간(커밋이 될 예정인 것들)
  (use "git add <file>..." to include in what will be committed)
        new.txt

# 커밋하기 위해 추가된 것은 없는데,untracked files는 존재한다.
# Working directory -> 파일 있어
# Staging area -> 파일 없어
nothing added to commit but untracked files present (use "git add" to track)
```

```bash
$ git status
On branch master
# 커밋될 변경사항들 (staging area)
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   new.txt
```

```bash
$ git status
On branch master
# Staging area (Staged O)
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   new.txt


# staged X (커밋을 위해)
# Working directory
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   2.txt

# 트래킹 X
# Working directory
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        hi.txt


```



## 용어

1) 커밋(버전)
2) 릴리즈
3) 커밋





## 실습

![과제](C:\Users\Owner\OneDrive\Desktop\과제.png)
