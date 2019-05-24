---
layout: post
title:  "HTTP ContentType 정리"
date:   2019-05-24
excerpt: "Just about everything you'll need to style in the theme: headings, paragraphs, blockquotes, tables, code blocks, and more."
tag:
- HTTP
- ContentType
comments: true
---

## HTTP 기술 방향
> HTML -> XML -> JSON형식으로 진행됨.

## Content-Type 의 종류
 - Multipart Related MIME 
 - XML Media 
 - Application 
 - Audio 
 - Multipart 
 - TEXT

## 선언 방식 
 - ASP  : <% Response.ContentType = "text/html" %>
 - JSP  : <%@ page contentType="text/html" %>
 - PHP  : PHP header("Content-Type:text/html");
 - Perl : "Content-type: text/html\n\n"

### Multipart Related MIME 타입
 - Multipart/related : 기본 형태
 - Application/X-FixedRecord : 
 
### XML Media 타입
 - text/xml : 
 - Application/xml : 
 - Application/xml-external-parsed-entity : 
 - Application/xml-dtd : 
 - Application/mathtml+xml : 
 - Application/xslt+xml : 
 
### Application 타입
 - Application/EDI-X12 : 
 - Application/EDIFACT : 
 - Application/javascript : 
 - Application/octet-stream : 
 - Application/ogg : 
 - Application/x-shockwave-flash : Adobe Flash 파일
 - Application/json : JavaScript Object Notation JSON / Defined in RFC 4627
 - Application/x-www-form-urlencode : HTML Form 형태 (저용량)
 - multipart/form-data : HTML Form 형태 (대용량)
 
### Audio 타입
 - audio/mpeg : MP3 / MPEG audio
 - audio/x-ms-wma : Windows Media Audio
 - audio/vnd.rn-realaudio : RealAudio...
 
### Multipart 타입
 - multipart/mixed : MIME E-mail
 - multipart/alternative : MIME E-mail
 - multipart/related : HTML E-mail
 - multipart/formed-data : 파일 첨부
 
### Text 타입
 - text/css :
 - text/html : 
 - text/javascript : 
 - text/plain : 
 - text/xml : 
 
 
 <a class = "btn btn-title" href="https://www.iana.org/assignments/media-types/media-types.xhtml#application"> 참고 사이트 </a> 
