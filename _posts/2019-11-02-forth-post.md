---
title: "Kokoa clone, challenge program 일지3"
date: 2019-11-02 11:14:28 -0400
categories: nomadChallenge
---
# kakao clone challenge 프로그램 일지 6

어느새 절반정도 달린 챌린지 프로그램!
그 사이에 나도 뭔가 많이 배운 것 같다?
처음 과제를 받았을 땐 정말 힘들었는데 이젠 검색과 응용력으로 잘 헤쳐나가는 중.
다음주는 실습파트이던데 내가 잘 해낼 수 있을까? 

# HTML ,CSS Code
**오늘은 2개의 과제를 제출했다**
![enter image description here](https://lh3.googleusercontent.com/BLQKXjE36u6SKM1_6JHu_kQvcJn1WK6GtCBQg2d4R-3SktY3QLkmcMZC0k4ZcrF-qIb02L0KBvcC "pre-loading page1")
**1. HTML 코드**
~~~
<!DOCTYPE  html>

<head>

<title  ="loading"></title>

<link  rel="stylesheet"  href="load.css">

</head>

<body>

<div  class="box">

<div  class="dot"></div>

<div  class="dot"></div>

<div  class="dot"></div>

</div>

</body>
~~~
**1-2. CSS 코드**
~~~
body{

background-color: rgb(128, 196, 196);

}

.box{

height: 800px;

display: flex;

justify-content: center;

align-items: center;

animation: spin 1s  infinite  ease-in-out;

  

}

.dot{

border-radius: 100%;

background-color: white;

width: 10px;

height: 10px;

margin: 10px;

}

  

@keyframes  spin{

0%{

transform: rotatez(0deg)

}

100%{

transform: rotatez(180deg);

}

}
~~~
![enter image description here](https://lh3.googleusercontent.com/P37Rau9koGF6B3vfUnjdStO-GIlrymfIk1DGhL3eScfKOXc2Re3FwyKPO6oNoAvS6MyOqHgWtie6 "pre-loading page2")

**2. HTML 코드**
~~~
<!DOCTYPE  html>

<head>

<title  =  "animaition2"></title>

<link  rel="stylesheet"  href="ani2.css">

</head>

<body>

<div  class="box">

<div  class="mini"></div>

<div  class="mini"></div>

<div  class="mini"></div>

<div  class="mini"></div>

<div  class="mini"></div>

</div>

</body>
~~~
**2-2. CSS 코드**
~~~
body{

background-color: rgb(47, 196, 201)

}

.box{

height:800px;

display: flex;

justify-content: center;

align-items: center;

  

}

.mini{

height:80px;

width:10px;

background-color: white;

margin:3px;

animation: extension 1s  infinite  ease-in-out;

  

}

  

@keyframes  extension{

0%{

transform: rotateX(0.2turn);

}

/* 70%{

transform: rotateX(0.1turn);

} */

100%{

trasnform: rotateX(0);

}

}

.box  .mini:nth-child(1){

animation-delay: .2s;

}

.box  .mini:nth-child(2){

animation-delay: 0.4s;

}

.box  .mini:nth-child(3){

animation-delay: 0.6s;

}

.box  .mini:nth-child(4){

animation-delay: 0.8s;

}

.box  .mini:nth-child(5){

animation-delay: 1s;

}
~~~

## 과제를 하며 느낀점
**역시 하면 된다!?**

Day 6의 과제를 받은 날짜는 토요일..
왠지 토요일이라 과제가 어려울 것 같다고 생각하며 [챌린지 사이트](https://challenges.nomadcoders.co/)에 접속했는데, 역시나..
*저걸 어떻게 구현하라는거야?*

일단 침착하게 엊그제 발매된 루이지멘션을 구입했다...
다운로드 시켜놓고 두시간동안 슬랙채널과 함께 코딩하다보니
생각보다 쉽게 과제가 풀렸다.

또 첫 날에 비해 검색하려는 의욕이 상승하였으며 (의욕+5)
과제가 2개이지만 첫번째 것을 완성하니 두번째 것도 생각보다 쉽게 해결됐다. (응용력+5)

역시 하면 되고 모르면 검색하면 된다. 화이팅!
이제 루이지멘션..이 아니라 월요일부터 다시 시작 될 챌린지 프로그램을 위해 예습하러 가야겠다.

> Written with [StackEdit](https://stackedit.io/).
