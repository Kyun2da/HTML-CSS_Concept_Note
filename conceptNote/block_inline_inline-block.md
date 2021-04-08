# block vs inline vs inline_block

위 세가지는 CSS 의 display 속성을 말한다.



#### block

block은 한 영역을 차지 하는 박스형태를 가지는 성질을 갖고 있다. 그렇기 때문에 기본적으로 block은 width값이 100%이다. 그리고 라인이 새로 추가된다는 것을 알 수 있다. 

- block은 height와 width 값을 지정 할 수 있다.
- block은 margin과 padding을 지정 할 수 있다.



#### inline

inline은 주로 텍스트를 주입 할 때 사용 되는 형태이다. 그렇기 때문에 기본적으로 block처럼 width값이 100%가 아닌 컨텐츠 영역 만큼 자동으로 잡히게 되며 라인이 새로 추가 되지 않는다. 높이 또한 폰트의 크기만큼 잡힌다.(line-height로 설정이 가능 하긴 하다.)

- width와 height를 명시 할 수 없다.
- margin은 위아래엔 적용 되지 않는다.
- padding은 좌우는 공간과 시각적인 부분이 모두 적용 되지만 위아래는 시각적으로는 추가되지만 공간을 차지 하지는 않는다.



#### inline-block

inline-block 은 말그대로 inline의 특징과 block의 특징을 모두 가진 요소이다. inline-block의 특징은 다음과 같다.

- 줄바꿈이 이루어지지 않는다.
- block처럼 width와 height를 지정 할 수 있다.
- 만약 width와 height를 지정하지 않을 경우, inline과 같이 컨텐츠만큼 영역이 잡힌다.

block 처럼 가로와 세로 크기를 설정 할 수 있으면서도, 새로운 줄에서 시작하지 않고, inline 처럼 다른 요소와 같은 라인에 배치되는 장점을 가지고 있다.