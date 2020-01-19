# flex

container(감싸는 부모박스)와

items(자식들 박스)로 크게 나뉘고 속성이 다르다

## container 적용 가능한 flex속성
+ display
    + flex
    + inline-flex

+ flex-flow(flex-direction,flex-wrap)
    + flex-direction : 주축
    row 수평 column 수직정렬
    + flex-wrap: 원래 크기를 갖으며 여러줄묶음(줄 바꿈)
    기본은 한줄이다.   
    wrap:item을 여러 줄로 묶음    
    riverse역방향

+ justify-conent
주축 정렬방법
    + flex-start 왼쪽 flex-end오른쪽 center가운데 space-between, space-around

+ align-content(교차 축 정렬방법wrap이 되어 여러줄일때만가능) 
    
    + 한줄일 경우 align-items(값 동일)
    + stretch auto일경우 자동으로 늘어남
    + :flex-start 위쪽 flex-end아래쪽으로 center가운데 space-between, space-around
~~~
한줄일경우 텍스트 중앙정렬
요소를 컨테이너화 시킨다
---display:flex;
---justify-content: center;
---align-items: center;
~~~

## item 적용 가능한 flex속성
+ order   
+ flex   
+ align-self   


