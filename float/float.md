## float사용과 해제

### flot
(요소를 띄운다,부유,수직,레이아웃구성)


### 값
float:방향(left; or right;)

### 특징

←←←←←←←←←←←←←
321(우측부터 쌓는다)

→→→→→→→→→→→→→
123(좌측부터쌓는다)

### 해제방법
flot은 해제를 꼭 해야하며 하지않으면 다음요소에 영향을 받는다. 끝나는 부분에 해제한다

1. 다음형제요소가 있으면 
형제요소에 clear:both;(해제한다 아무방향)을 사용

2. 부모요소에 overflow:hidden(요즘에는사용X)

3. ★부모요소에 clearfix클래스를 추가하여 해제★

~~~
.clearfix:after{}
 (부모 클리어픽스클래스안에 있는 요소만 만지정)

부모영역(.clearfix)안에있는 자식들만 내가 해제시켜줄게
우리 자식들만 적용이된단다
너네집 가서 clearfix 사달라고하렴

.clearfix:after{
    content:"";
    clear:both;
    display:block;
}
공식이라고 생각하자
~~~

주의

+ clearfix 클래스를 추가하는 부모요소의 자식요소는
무조건 float 상태만 있어야한다(float자식모임)


---

다시 정리

[09 CSS Clear속성 이해와 활용(웹퍼블리셔를 위한 웹표준, 웹접근성 실무기초)](https://www.youtube.com/watch?v=641i0NjaqBs&list=PL_6yF2upGJYu-mdzvejWuz6zLd5EOFQKf&index=9)

~~~
<ul>
    <li>홈 > </li>
    <li>기업소개 > </li>
    <li>인사말 > </li>
</ul>

li를 left로 띄우고 ul에 right로 우측으로 보낸다

~~~

해제방법

1. 다음으로 오는 요소에 clear:both를 사용하거나 
없을경우 br(block)을 만들고 clear속성을 적용하여 해제
(float을 적용하면 부모요소 높이는 사라진다)

2. 가상선택자사용(clearfix:after)

    + 부모요소에 클래스 .claerfix(class name)을 추가한다
(다중선택자)

~~~
.clearfix:after{

    content:"";            가상의 span(inline)만든다
    display:block;         성질을 block으로 바꾼다
    clear:both;            clear를 넣는다.
}

~~~






    