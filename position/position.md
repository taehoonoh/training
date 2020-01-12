# position
:위치 지정방법의 유형(기준)을 배치

## 속성 값

+ relative : 요소자신을 기준 배치 
+ absoulute : 위치상 부모요소를 기준 배치
+ fixed : 뷰포트를 기준 배치
+ sticky : 스크롤 기준 배치

+적용 후 추가 속성으로 위치 값 조정

top,right,bottom,right   
:요소 position 기준에 맞는 (방향)에서의 거리

### relative
:자기 자신을 기준으로 움직인다(마치 분신술)

+ 영혼은 그 자리에 있어서 
다른 형제요소에 위치에 영향을 끼친다

### ★absoulute
:부모요소(위치상부모)을 기준으로 움직인다

부모-자식 position 값 확인 적용
~~~
.parent{
            width:400px;
            height: 300px;
            border:4px dashed gray;
            position: relative;
            
        }

        .absolute{
            bottom:50px;
            right:10px;  
            position: absolute;     
        }
~~~

★자식요소에 position:absolute를 적용한다음 
  
★부모요소에도 position이 적용되어있는지 확인후   
부모요소도 포지션 적용(보통 position:relative;)

적용순서(부모요소에 포지션이 없으면)   
+ 부모요소>조상요소>body>html>윈도우객체(뷰포트)


