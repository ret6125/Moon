---
layout: post
title:  "블로그 만들기(환경설정)"
date:   2019-05-14
excerpt: "Just about everything you'll need to style in the theme: headings, paragraphs, blockquotes, tables, code blocks, and more."
tag:
- markdown 
- syntax
- sample
- test
- jekyll
comments: true
---

# Jekyll configuration

### markdown: kramdown
// kramdown : markdown 업데이트된 버전
<hr/>

##### text highlighter 강조 : 2016.02월 이후 rouge만 지원
highlighter: rouge

##### 페이지당 보여지는 max갯수 설정
paginate: 10

##### 언어 설정
language: 'en-uk'

##### 없을 경우 Google Search Console에서 sitemap.xml 정상적인 생성 불가
##### 또한 disqus( 댓글 시스템)를 이용하기 위해서도 필요.
##### 자신의 github page url을 입력 ( https://yourID.github_id.github.io 형식 )
url: https://ret6125.github.io


baseurl: /

## Website info
##### 자신의 blog title.
title: IT Blog

##### blog home에 표시될 blog에 대한 설명.
description: Development & Technical Training

##### blog home의 cover image.
cover: assets/built/images/blog-cover.png


logo:
logo_dark:

##### favicon image
favicon: assets/built/images/favicon.jpg

##### 운영 blog url
production_url: https://moon9342.github.io/

##### blogmaker(jekyll source folder)의 github repository
source_url: https://github.com/moon9342/GitHubPageMaker/


## Social info
##### Navigation bar link 유무
navigation: True

##### subscriber 기능을 사용 유무
##### subscriber 기능 -> lunr.js를 이용한 검색 기능으로 대체
##### 검색기능 대체 기능
##### `_includes/subscribe-form.html` 파일의 수정이 필요
subscribers: True

##### twitter username
twitter:
##### facebook username
facebook:


## Disqus
##### 온라인 댓글 시스템. 댓글 기능을 사용 유무
disqus: True
##### disqus shortname을 입력 ( disqus username (X) )
disqus_shortname: sunghoons-blog


## Google Analytics
##### Google Analytics을 사용할 경우 GA tracking identifier를 입력
google_analytics:  ##### replace with your GA tracking identifier


## Permalinks
permalink: /:title
##### permalink: /author/:author
##### permalink: /tag/:title
##### 각각의 post에 고정주소를 어떤 방식으로 할당할 것인지를 결정
##### 이 값을 바꾸면 작성한 포스트의 저장위치나 파일이름이 변경된다.

##### gems and other configs
plugins: [jekyll-paginate, jekyll-feed, jekyll-gist]

feed:
  path: feed.xml

##### Travis-CI 설정입니다.
safe: False
lsi: False

##### travis-ci와 연동하는 github의 username
username: moon9342
##### travis-ci와 연동하는 github의 repository이름
repo: GitHubPageMaker
##### ex> https://github.com/<username>/<repository>

##### branch명
branch: master


relative_source: 

##### repository : https://username.github.io
##### compile 결과 폴더 (운영하는 블로그 내용이 컴파일 되는 파일등..)
##### github repository에 push 되는 파일이며, Travis-CI를 이용할 예정이면 이 부분을 git submodule을 github repository에 연결해야 됨.
destination: ./output/

##### exclude는 Jekyll컴파일 시 destination에 포함될 필요가 없는것들을 명시한다. (node_modules는 포함해야 함.)
exclude:
  - README.md
  - Rakefile
  - Gemfile
  - Gemfile.lock
  - changelog.md
  - "*.Rmd"
  - vendor
  - .travis.yml
  - node_modules
