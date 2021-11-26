### 소프트웨어학부 20213032 윤홍현

## git에 저장소 만들기

## 이미 만들어진 Lanyon 테마 웹사이트에서 시작하기
1. Lanyon 테마의 원격 저장소 내용을 다운받는다.   
[Lanyon 원격 저장소 링크](https://github.com/poole/lanyon)
2. hongbuly.github.io 라는 저장소에 해당 내용을 넣는다.

## _config.yml 파일 수정하기
#### 탬플릿의 dummy 정보가 아닌 나의 웹사이트 정보로 교체하는 일이 필요하다.
<pre>
<code>
# Setup
title:               Hongbuly
tagline:             'Hongbuly blog'
description:         'This blog is written by one of the kookmin univer's student.'
url:                 https://hongbuly.github.io
# baseurl:             ''
paginate:            5
permalink:           pretty
comments:            true

# About/contact
author:
  name:              Honghyun Youn
  url:               https://hongbuly.github.io
  email:             hongbulys@gmail.com

# Gems
plugins:
  - jekyll-paginate

# Custom vars
version:             1.1.0
google_analytics_id: #UA-XXXX-Y
comment:
  provider: "disqus"
  disqus:
    shortname: "hongbuly"

</code>
</pre>
