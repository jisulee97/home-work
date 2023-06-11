### html 코드 설명

가장 바깥쪽을 div 태그로 감싸고 관련 사이트를 h3으로 준 다음
안쪽을 content로 감싸서 그 안에 ul과 li 태그로 리스트를 만들어서 디자인 하였다.

### css 코드 설명
```
 <div class="site-box">
 ```
전체 크기와 안쪽 패딩을 주었고 배경색은 linear-gradient 를 주어 그라데이션 효과를 주었다

```
<h3>관련 <span>사이트</span><h3>
```
h3는 블록 요소인데 '관련' 과 '사이트'에 글자색이 달라서 '사이트' 부분을 span 요소로 묶고
display: inline-block 을 주어 줄바꿈이 일어나지 않도록 설정하였다

```
<div class="content">
```
overflow-y: hidden 속성을 주어 y축으로 가려지지 않는 li들을 가리는 속성을 활용했고
안에 리스트들을 움직이기 위해 부모인 이 곳에 position: relative 속성을 주었고 0.5s의 시간을 주었다
hover 시에는 0.4초동안 200px이 늘어나도록 설정

```
<ul class="content-list">
```
position: relative 를 주어 위쪽에 고정시키기 위해 top:0 값을 주었고 content와 다르게 움직어야 하기 때문에 0.5초의 딜레이 시간을 주었다
hover 시에는 부모인 content로 부터 top: 15px 움직이고 움직이면서 위치가 아래로 내려가기 때문에 위치를 맞추기 위해 height는 180px로 늘렸다