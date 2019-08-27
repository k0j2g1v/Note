# Github 특강 1일차

## Git hub와 연결
#### Repositories 생성	
 ```cmd
 k0j2g1v.github.io 
 ```
   형식은 (자신의 GitHub 닉네임).github.io에 맞춘다

#### Github와 Git Bash와 연결
```cmd
 - git config --global user.email "k0j2g11@naver.com"
	#Github의 이메일 입력
 - git config --global user.name "Choi Jea Bum"
	#자신의 쓰고자하는 닉네임 입력
```

#### Github에 파일 올리기

##### init > add > commit > push 순으로 진행된다.
```cmd
- git init
	#git 연결에대한 초기설정
	#제 디렉토리를 git의 저장소로 만든다
- git status
	#파일의 상태를 확인할때 사용된다
- git add .(현제 위치 전부)  or  (파일 이름)
	#commit을 하기위해 파일을 추가해주는 명령어이다.
- git commit -m " 메 세 지 "
	#add를 통해 추가된 파일이나 내용을 메세지와 함께 커밋한다
- git remote add origin + URL 
	##GitHub에 Repository가 생성되어 있어야한다.
	#원격 저장소를 손쉽게 추가하는 방법이다.
	#URL 자리에 자신의 Repositorie의 클론주소를 넣어주면된다
- git push -u origin master
	#push는 마지막 commit사항을 Git Repository에 올린다는 뜻이다
	#origin은 로컬저장소이고 master은 branch명이다
- git pull origin master
	#Git Repository로부터 최근의 데이터를 받아온다.

#기타 명령어
 - git log -(숫자)  #원하는 줄만큼의 로그창을 출력한다
 - git log --oneline #로그창을 보기쉽게 한줄로 표시해준다.
 - git checkout (해시코드) #각각 커밋에대한 고유키(5~6자리)를 입니다
	 		              #해당 위치로 이동
```
## Branch
- 독립적으로 작업을 진행하기위한 개념이다. 
- 각각의 브렌치는 서로에게 영향을 받지 않고 작업할 수 
  있도록해주는 일시적인 기능이다.
```cmd
- git branch (name)  #새로운 branch생성
- git checkout (name)   #해당 branch로 이동
- git checkout -b new   #new라는 branch생성 및 이동
- git branch -d new     #new라는 branch삭제
```

