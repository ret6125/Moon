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
## 1XX - 정보응답 : request를 받고 처리중에 있음
> 일반적으로 서버 -> 클라이언트로 보내지 않음
<hr/>

### 100 : Continue
### 101 : Switching Protocol (WebSocket 등에서 사용)
### 102 : Processing

<hr/>
## 2XX - 성공 : request 처리 완료
> 일반적으로 200 / 206 사용
<hr/>

### 200 : OK
> request가 정상적으로 받은 상태

### 201 : Created
> request가 성공적으로 처리, 리소스가 생성된 상태

### 202 : Accepted
> request가 성공적으로 받았으나, 서버에서 처리되지 않은 상태

### 203 : Non-Authoritative Information
> response meta Data가 origin 서버와 일치하진 않지만, 로컬 / 서드파티 복사본이 모아져있는 상태

### 204 : No Content
> request가 성공적으로 받았으나, 컨텐츠를 제공하지 않는 상태

### 205 : Reset Content
> request가 성공적으로 받았으나, 컨텐츠를 표시하지 않은 상태 (재설정 요구함.)

### 206 : Partial Content
> request가 성공적으로 받았으나, 컨텐츠의 일부분만 제공하는 상태 (ex> 일정 범위로 쪼개서 다운로드 )

### 207 : Multi-Status
> 여러 리소스가 여러 상태 코드인 상황이 적절한 경우에 해당 정보를 전달하고 있는 상태

### 208 : Already Reported (DAV 사용)
> 응답속성으로 동일 컬렉션으로 바인드된 복수의 내부 멤버를 반복되는것을 방지하기 위한 상태

### 226 : IM Used
> 인스턴스 조작이 적용된 상태

