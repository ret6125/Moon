---
layout: post
title:  "HTTP Error Code 정리"
date:   2019-06-04
excerpt: "Error Code 정리 내용"
tag:
- HTTP
- ContentType
comments: true
---

<hr/>
## 1XX - 정보응답 : request를 받고 처리중에 있음 (일반적으로 서버 -> 클라이언트로 보내지 않음)
<hr/>

### 100 : Continue
### 101 : Switching Protocol (WebSocket 등에서 사용)
### 102 : Processing

<hr/>
## 2XX - 성공 : request 처리 완료
<hr/>

### 200 : OK
| request가 정상적으로 받은 상태
### 201 : Created
| request가 성공적으로 처리, 리소스 만들어진 상태
### 202 : Accepted
| request가 성공적으로 받았으나, 서버에서 처리되지 않은 상태
### 203 : Non-Authoritative Information
| ??
### 204 : No Content
| request가 성공적으로 받았으나, 컨텐츠를 제공하지 않는 상태
### 205 : Reset Content
| request가 성공적으로 받았으나, 컨텐츠를 표시하지 않은 상태 (재설정 요구함.)
### 206 : Partial Content
| request가 성공적으로 받았으나, 컨텐츠의 일부분만 제공하는 상태 (ex> 다운로드 범위지정[자동])
### 207 : Multi-Status
| ??
### 208 : Already Reported
| ??
### 2226 : IM Used
| ??
