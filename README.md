### 소프트웨어학부 20213032 윤홍현

## git에 저장소 만들기
#### Github 사이트에 들어가서 왼쪽 상단 new 버튼을 눌러 새로운 저장소를 만든다.
<img src="images/git01.png" width="60%" height="60%">

#### Repository 이름을 `<username>.github.io` 로 하고 Public으로 생성한다.   
###### 지금 사진은 이미 만들어져 있어서 그렇다. 처음 만들면 정상적으로 생성할 수 있다.
<img src="images/git02.png" width="60%" height="60%">

#### git을 설치하고 HTTPS 형식으로 git clone을 한다. [Git 설치 링크](https://git-scm.com/downloads)
###### Github Desktop을 설치하면 GUI로 git을 관리할 수 있어 CLI보다 친근하다.
<img src="images/git03.png" width="60%" height="60%">

#### 원하는 디렉터리로 이동하고 git bash를 실행시킨다. 그리고 명령어로 git clone <HTTPS 주소> 라고 적는다.

    $ git clone https://github.com/hongbuly/hongbuly.github.io.git

#### 이제 git <명령어>를 통해서 git을 관리할 수 있다.
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

## 이미 만들어진 Lanyon 테마 웹사이트에서 시작하기
1. Lanyon 테마의 원격 저장소 내용을 다운받는다.   
[Lanyon 원격 저장소 링크](https://github.com/poole/lanyon)
2. hongbuly.github.io 라는 저장소에 해당 내용을 넣는다.

## _config.yml 파일 수정하기
#### 탬플릿의 dummy 정보가 아닌 나의 웹사이트 정보로 교체하는 일이 필요하다.   가장 중요한 것은 url에 나의 웹주소를 적고, baseurl을 주석처리를 해야 원하는 결과가 잘 나온다.
<pre>
<code>
# Setup
title:               Hongbuly # 페이지 상단에 뜨는 이름
tagline:             'Hongbuly blog' # title 옆에 뜨는 이름
description:         'A reserved <a href="https://jekyllrb.com" target="_blank">Jekyll</a> theme that places the utmost gravity on content with a hidden drawer. Made by <a href="https://twitter.com/mdo" target="_blank">@mdo</a>.'
url:                 https://hongbuly.github.io # 웹주소
# baseurl:             ''
paginate:            5
permalink:           pretty
comments:            true # 댓글 허용

# About/contact
author:
  name:              Honghyun Youn
  url:               https://hongbuly.github.io
  email:             hongbulys@gmail.com

# Gems
plugins:
  - jekyll-paginate

# Custom vars 댓글 기능
version:             1.1.0
google_analytics_id: #UA-XXXX-Y
comment:
  provider: "disqus"
  disqus:
    shortname: "hongbuly"

</code>
</pre>
