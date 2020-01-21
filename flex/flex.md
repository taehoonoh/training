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

+ justify-conent ★
주축 정렬방법
    + flex-start 왼쪽 flex-end오른쪽 center가운데 space-between, space-around

+ align-content(교차 축 정렬방법wrap이 되어  여러줄일때만가능) 
    
    + 한줄일 경우 align-items(값 동일) ★
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
+ order순서:음수도가능

+ flex : 증가 너비 기본(★1일때는 basis 0이된다)

    + flex-grow:증가너비 비율(기본0)

    + flex-shrink:감소너비 비율(기본1)

    + flex-basis:(공간배분전)기본 너비를설정(기본auto)

+ align-self:교차 축에서개별 item 정렬방법   
(align-item 값과 같다 
보다 우선적용 auto는 상속받는다)
