### 소프트웨어학부 20213032 윤홍현

## git에 저장소 만들기
#### Github 사이트에 들어가서 왼쪽 상단 new 버튼을 눌러 새로운 저장소를 만든다.
<img src="images/git01.png", width="30%" height="30%">

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
