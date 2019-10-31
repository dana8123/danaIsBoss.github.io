---
title: "Kokoa clone, challenge program 일지"
date: 2019-11-01 01:22:28 -0400
categories: HTML
---
# 챌린지 두번째 코딩문제를 푸는 도중 깨달은 것

## 1. Flex는 항상 적용하고자하는 컨테이너의 상위 컨테이너에 넣을 것
- 처음에는 가장 상위 컨테이너에 적용시키면 하위 컨테이너에도 다 적용될 줄 알았는데 그게 아니었다. 뭐든 flex를 적용시키고 싶다면 인접한 상위 컨테이너에 넣어야하는건가? 생각해봐야겠다.

## 2. 검색을 좀 더 꼼꼼히 할 것. 
-가장 하위의 회색 box들의 패딩 간격이 일정하지 않아 패딩을 넣으려했으나 과제의 요구사항에서 패딩과 마진값을 적용하지말라는 조건을 발견.
 justify-contentd태그에 대해 검색하였으나 답을 찾지 못했음. 그러나 슬랙 채널에 질문했을 때 evenly-space라는 태그도 있다는 것을 친절한 누군가의 답변으로 알게됨. 결국 문제가 풀렸음! 야호! 검색을 좀 더 열심히 하자!

# flex를 이용하여 과제를 풀자.
## HTML
~~~
<!DOCTYPE html>
<html>
  <head>
    <title>Kokoa Tribe</title>
    <meta charset="UTF-8" >
    <link rel="stylesheet" href="styles3.css" >
  </head>

  <body>
    <div class="mother">
      <div class="pinkbox">
        <div class="box"></div>
        <div class="box"></div>
        <div class="box"></div>
       </div> 
    </div>    
  </body>
</html>
~~~
## CSS 
~~~

body{
    padding : 0px;
    margin : 0px;
    background-color: skyblue;
    width: 1500px;
}
h1{
    color: white;
}
.mother{
    display: flex;
}
.bar{
    display: flex;
    align-items: flex-start;
    width:100%;
    height:200px;
    background-color: rgb(235, 119, 98);
    position: fixed;
    

}
.column{
    justify-content : flex-start;
    height:1500px; 
    width: 400px;
    background-color: yellow;
    border: 4px solid rgb(158, 157, 157);
}
.mainbox{
    width: 1500px;
    height:300px;
    background-color: skyblue;
    
}
.small{
    width: 30px;
    height: 20px;
    background-color: yellowgreen;
    justify-content: center;


}

~~~    

### 여담으로, 블로그를 만들고 꾸준히 글을 쓰려고 노력중이다. 이것저것 다 하려니 뭐 하나는 꼭 빠뜨리게된다. 그래도 화이팅!
또, 왜 내 포스트는 마크다운 문법이 적용되다가 마는가?? 저 샾(#)뭐냐고..
헐 알았다. #쓰고 바로 한 칸 띄워야 적용되네!


