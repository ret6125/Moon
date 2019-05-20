---
layout: post
title:  "블로그 만들기(환경설정)"
date:   2019-05-20
excerpt: "Git hub 블로그 환경설정 정리"
tag:
- blog
- markdown 
- syntax
- sample
- jekyll
comments: true
---

# Jekyll configuration
<hr/>

#### markdown: kramdown
> kramdown : markdown 업데이트된 버전


#### highlighter: rouge
>  text highlighter 강조 : 2016.02월 이후 rouge만 지원

#### paginate: 10
>  페이지당 보여지는 max갯수 설정

#### language: 'en-uk'
>  언어 설정

#### url: https:>ret6125.github.io
>  없을 경우 Google Search Console에서 sitemap.xml 정상적인 생성 불가
>  또한 disqus( 댓글 시스템)를 이용하기 위해서도 필요.
>  자신의 github page url을 입력 ( https:>yourID.github_id.github.io 형식 )

#### baseurl: /

<hr/>
## Website info
<hr/>
#### title: IT Blog
>  자신의 blog title.

#### description: Development & Technical Training
>  blog home에 표시될 blog에 대한 설명.

#### cover: assets/built/images/blog-cover.png
>  blog home의 cover image.

#### logo:
#### logo_dark:

#### favicon: assets/built/images/favicon.jpg
>  favicon image

#### production_url: https:>moon9342.github.io/
>  운영 blog url

#### source_url: https:>github.com/moon9342/GitHubPageMaker/
>  blogmaker(jekyll source folder)의 github repository

<hr/>
## Social info
<hr/>
#### navigation: True
>  Navigation bar link 유무

#### subscribers: True
>  subscriber 기능을 사용 유무
>  subscriber 기능 -> lunr.js를 이용한 검색 기능으로 대체
>  검색기능 대체 기능
>  `_includes/subscribe-form.html` 파일의 수정이 필요

#### twitter:
>  twitter username

#### facebook:
>  facebook username

<hr/>
## Disqus
<hr/>
#### disqus: True
>  온라인 댓글 시스템. 댓글 기능을 사용 유무

#### disqus_shortname: sunghoons-blog
>  disqus shortname을 입력 ( disqus username (X) )

<hr/>
## Google Analytics
<hr/>

#### google_analytics:
>  Google Analytics을 사용할 경우 GA tracking identifier를 입력

<hr/>
## Permalinks
<hr/>

#### permalink: /:title
>  permalink: /author/:author
>  permalink: /tag/:title
>  각각의 post에 고정주소를 어떤 방식으로 할당할 것인지를 결정
>  이 값을 바꾸면 작성한 포스트의 저장위치나 파일이름이 변경된다.


#### plugins: [jekyll-paginate, jekyll-feed, jekyll-gist]
>  gems and other configs

#### feed:
#### path: feed.xml
>  Travis-CI 설정

#### safe: False
#### lsi: False

#### username: moon9342
>  travis-ci와 연동하는 github의 username

#### repo: GitHubPageMaker
>  travis-ci와 연동하는 github의 repository이름
>  ex> https:>github.com/<username>/<repository>

#### branch: master
>  branch명

#### relative_source:
>  repository : https:>username.github.io
>  compile 결과 폴더 (운영하는 블로그 내용이 컴파일 되는 파일등..)
>  github repository에 push 되는 파일이며, Travis-CI를 이용할 예정이면 이 부분을 git submodule을 github repository에 연결해야 됨.
destination: ./output/


### exclude:
  - README.md
  - Rakefile
  - Gemfile
  - Gemfile.lock
  - changelog.md
  - "*.Rmd"
  - vendor
  - .travis.yml
  - node_modules
>  exclude는 Jekyll컴파일 시 destination에 포함될 필요가 없는것들을 명시한다. (node_modules는 포함해야 함.)
