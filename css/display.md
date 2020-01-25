# block,inline,inline-block

여기 있는 내용과 공부한 내용을 더하여 정리함
https://poiemaweb.com/ 
## block 레벨 요소 특성
(div h1 ~ h6 p ol ul li hr table form)

+ 항상 새로운 라인에서 시작한다.

+ 수직으로 쌓인다

+ 화면 크기 전체의 가로폭을 차지한다   
(최대가로너비) (width: 100%; height:0;로 시작) 

+ width, height, margin, padding   
(크기를 지정할수있다.)

+ block 레벨 요소 내에 inline 레벨 요소를 포함할 수 있다

+ 레이아웃을 잡을때

## inline 레벨 요소 특성
(span a strong img br input select textarea button)

+ 새로운 라인에서 시작하지 않으며 문장의 중간에 들어갈 수 있다. 즉, 줄을 바꾸지 않고 다른 요소와 함께 한 행에 위치한다.

+ 수평으로 쌓인다.

+ content의 너비만큼 가로폭을 차지한다.(필요한만큼)

+ width, height, margin, padding top bottom X(width:0; height:0;)
상, 하 여백은 line-height로 지정한다.

+ inline 레벨 요소 뒤에 공백(엔터, 스페이스 등)이 있는 경우, 정의하지 않은 space(4px)가 자동 지정된다.

+ inline 레벨 요소 내에 block 레벨 요소를 포함할 수 없다. inline 레벨 요소는 일반적으로 block 레벨 요소에 포함되어 사용된다.

+ 텍스트를 잡는 용도

## inline-block 레벨 요소

+ block과 inline 레벨 요소의 특징을 모두 갖는다. 

+ inline 레벨 요소와 같이 한 줄에 표현되면서 width, height, margin 프로퍼티를 모두 지정할 수 있다.

+ 기본적으로 inline 레벨 요소와 흡사하게 줄을 바꾸지 않고 다른 요소와 함께 한 행에 위치시킬 수 있다.

+ block 레벨 요소처럼 width, height, margin, padding 프로퍼티를 모두 정의할 수 있다. 

+ 상, 하 여백을 margin과 line-height 두가지 프로퍼티 모두를 통해 제어할 수 있다.

+ content의 너비만큼 가로폭을 차지한다.

+ inline-block 레벨 요소 뒤에 공백(엔터, 스페이스 등)이 있는 경우, 정의하지 않은 space(4px)가 자동 지정된다. 
    + 해결방법:부모요소에 font-size:0을 준다



