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

## 이미 만들어진 Lanyon 테마 웹사이트에서 시작하기
1. Lanyon 테마의 원격 저장소 내용을 다운받는다.   
[Lanyon 원격 저장소 링크](https://github.com/poole/lanyon)
2. hongbuly.github.io 라는 저장소에 해당 내용을 넣는다.

## _config.yml 파일 수정하기
#### 탬플릿의 dummy 정보가 아닌 나의 웹사이트 정보로 교체하는 일이 필요하다.  
#### 가장 중요한 것은 url에 나의 웹주소를 적고, baseurl을 주석처리를 해야 주소창에 url을 적었을 때 결과가 잘 나온다.
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

## sidebar.html 파일 수정하기
#### 왼쪽 사이드바에 Download, Github project가 있는데 불필요해서 다음과 같은 코드를 주석처리 해주었다.
<pre>
<code>
<a class="sidebar-nav-item" href="{{ site.github.repo }}/archive/v{{ site.version }}.zip">Download</a>
<a class="sidebar-nav-item" href="{{ site.github.repo }}">GitHub project</a>
</code>
</pre>

## _posts 디렉토리에 post 글 추가하기
#### 글을 쓰고 싶을 때, _posts 디렉토리에 "년도-월-일-이름.md"로 파일을 생성해서 작성해야 한다.
##### "-"를 빼먹거나 형식이 틀리지 않게 주의해야 한다.

    2021-11-25-Git&Github.md

#### 파일 상단에 다음과 같은 내용을 쓴 다음 글을 써야 한다.
<pre>
<code>
---
layout: post
title: Git&Github # 글 제목
date: 2021-11-25 16:30:59 +0900 # 날짜와 시간
categories: jekyll update
comments: true # 댓글 허용
---
</code>
</pre>

## 댓글 기능 추가하기
#### post 글에 Disqus를 이용해 간단히 추가할 수 있다.
#### 먼저 회원가입을 한다.
<img src="images/disqus01.png" width="60%" height="60%">
<img src="images/disqus02.png" width="60%" height="60%">
