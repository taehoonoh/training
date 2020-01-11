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








    