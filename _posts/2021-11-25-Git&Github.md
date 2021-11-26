---
layout: post
title: Git&Github
date: 2021-11-25 16:30:59 +0900
categories: jekyll update
comments: true
---

## Git이란?   
깃은 컴퓨터 파일의 변경사항을 추적하고, 여러 명의 사용자들 간에 해당 파일들의 작업을 조율하기 위한 **분산 버전 관리 시스템**입니다.   

#### 원하는 Local repository 디렉토리에서 git bash를 실행시킨 후, git <명령어>를 통해서 git을 관리할 수 있다.
<img src="images/git04.png" width="60%" height="60%">

#### 현재 Git 상태 확인 명령어

    $ git status

#### commit을 위해 Staging Area에 파일을 올리는 명령어

    $ git add README.md

#### commit 메시지를 적고 commit 하는 명령어

    $ git commit -m "add README.md"

#### commit 기록 확인하기

    $ git log

<hr/>

#### 개발을 할 때 기능을 추가하거나 에러를 처리하는 등 다양한 일들을 할 수 있다.   그럴 때 코드의 흐름을 분산시켜 더욱 효율적인 개발을 가능하도록 해주는 개념이 `Branch`이다.

#### branch 생성하는 명령어

    $ git branch <branch_name>

#### 현재 작업중인 branch 전환하는 명령어

    $ git checkout <branch_name>

#### branch를 main에 병합시키는 명령어

    $ git merge <branch_name>

#### branch 삭제하는 명령어

    $ git branch -d <branch_name>