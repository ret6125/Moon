---
layout: post
title:  "Clean Swift Architecture"
date:   2019-06-11
excerpt: "iOS Clean Architecture"
tag:
- HTTP
- ContentType
comments: true
---

<hr/>

Clean Architecture : 로보트 ?? 마틴 발명

> 원형의 다이어그램으로 되어 있다
> 밖은 하위 안쪽은 상위레벨의 메커니즘(정책)으로 구성되어있으며, 관심 책임으로 나뉠 수 있다.
> 상위레벨은 하위레벨의 디펜더시가 없어야 한다.


## VIP Cycle : ViewController ->  Internador -> Presenter -> ViewController
<hr/>
### Logic
 * ViewController : Display Logic
 * Internador : Business Logic
 * Presenter : Presnettaion Logic
 
### Protocol (구조체) : 레퍼런싱 
 * ViewController ->  Internador : Request
 * Internador -> Presenter : Response
 * Presenter -> ViewController : View Model
   
 
 
