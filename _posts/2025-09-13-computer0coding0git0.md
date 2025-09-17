---
layout: post
title: simple use git command
author: ZeroDoc
name: Zero
date: 2025-09-13 20:00:00 +0900
categories: [Computer,Git]
tags: []     # TAG names should always be lowercase, 띄어쓰기도 금지
comments: true
pin: false
toc: true
---
## Git & Github
- Git 설치하기   
 https://git-scm.com/downloads

- GitHub에 Repository 만들기
 https://github.com/

## Repository 생성 후
## GitHub에 접속하여 작업할 Repository에서 Code라고 써진 곳을 클릭하여 주소를 복사합니다. (xxxxx.git)

> " git init, add, commit  "

- Git을 받으면 설치되는 Git Bash를 실행시켜줍시다.   
(작업/업로드 할 파일 폴더 안에서 우클릭 - Git Bash Here)   
또는 프롬프트에서 해당 경로로 진입

## 처음일 경우 초기 설정(사용자정보)을 해주어야 합니다.   
- git config –global user.name [GitHubName]   
- git config –global user.email [GitHubEmail]

```
작업폴더에서

git init

그럼 해당 폴더에 .git 파일이 생성됩니다.   
레포에 업로드 할 작업 내용을 추가   

git add .    

뒤에 있는 .은 모든 파일을 의미.   
특정 파일이나 폴더를 업로드 하고 싶다면 git add XXX.txt와 같이 입력하면 됩니다.   

그 다음   

git commit -m “message”

뒤에 있는 “message”는 로그입니다. 어떤 작업을 했는지 짧게 기록하기
```
>작업내용을 묶어서(add), 설명서를 포함(commit), 업로드(push) 한다.   

첫 push일 경우   

git push -u origin master   
(현재20250901, master -> main 변경됨)   

여기서 origin은 아까 복사한 경로를 붙여넣기

처음일 push일 경우 GitHub Login 페이지가 뜨는데 email, password, username을 칸에 맞게 입력해주시면 됩니다.

이후 동일 작업일 시, git push 만 해도 업로드 됨   
: 혼자 쓸거니 심오한 사용법은 패~~~ 스~~~~  !!!!!

>요약   
>처음일 경우 초기 설정(사용자정보)을 해주어야 합니다.      
>- git config –global user.name [GitHubName]   
>- git config –global user.email [GitHubEmail]   
>작업폴더에서   
>- git add.   
>- git commit -m "message"   
>처음 업로드 시   
>- git push -u  origin main   
>(origing: repo경로.git, main: 브랜치명)   
>(이후는 git push 만 해도 업로드 됨)   
```
