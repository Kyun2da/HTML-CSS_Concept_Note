# CSS Colors

색깔은 미리정의된 색깔이름들을 사용하거나 RGB, HEX, HSL, RGBA, HSLA 값을 사용한다.

------

## CSS 색깔 이름

CSS에서는 색깔은 아래와 같은 색깔 이름을 사용한다.

Tomato

Orange

DodgerBlue

MediumSeaGreen

Gray

SlateBlue

Violet

LightGray



CSS/HTML은 140개의 표준 색상 이름을 지원한다. 다음의 링크를 참조하자 [140 standard color names](https://www.w3schools.com/colors/colors_names.asp).

------

## CSS 배경 색

너는 HTML 엘리먼트의 배경색을 지정할 수 있다.

### 예제

```html
<h1 style="background-color:DodgerBlue;">Hello World</h1>
<p style="background-color:Tomato;">Lorem ipsum...</p>
```



------

## CSS 텍스트 색상

너는 텍스트의 색상또한 지정할 수 있다.

### 예제

```html
<h1 style="color:Tomato;">Hello World</h1>
<p style="color:DodgerBlue;">Lorem ipsum...</p>
<p style="color:MediumSeaGreen;">Ut wisi enim...</p>
```

------

## CSS 테두리 색상

너는 테두리의 색상을 지정할 수 있다.

### 예제

```html
<h1 style="border:2px solid Tomato;">Hello World</h1>
<h1 style="border:2px solid DodgerBlue;">Hello World</h1>
<h1 style="border:2px solid Violet;">Hello World</h1>
```



------

## CSS 색상값

CSS에서 RGB, HEX, HSL, RGBA, HSLA 값을 사용하여 색상을 조정할 수있다.

### 예제

```html
<h1 style="background-color:rgb(255, 99, 71);">...</h1>
<h1 style="background-color:#ff6347;">...</h1>
<h1 style="background-color:hsl(9, 100%, 64%);">...</h1>

<h1 style="background-color:rgba(255, 99, 71, 0.5);">...</h1>
<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">...</h1>
```



## CSS RGB 값

CSS에서 RGB값으로의 색상은 다음과 같은 공식을 사용한다.

rgb(*red,* *green*, *blue*)

### 예제

rgb(255, 0, 0)

rgb(0, 0, 255)

rgb(60, 179, 113)

rgb(238, 130, 238)

rgb(255, 165, 0)

rgb(106, 90, 205)



회색도 3개의 색 원소로 지정할 수있다. ( 회색은 3개의 색이 같음)

### 예제

rgb(0, 0, 0)

rgb(60, 60, 60)

rgb(120, 120, 120)

rgb(180, 180, 180)

rgb(240, 240, 240)

rgb(255, 255, 255)



------

## CSS HEX 값

CSS에서 HEX 색상은 다음과같은 형태로 표현될 수있다

\#*rrggbb*

rr은 빨강, gg는 초록, bb는 파랑이다. 이 값들은 00에서  ff의 값을 갖는다.( 이는 10진수에서 0~255와 같음)

예를들어 #ff0000은 빨간색으로 보여지는데 왜냐하면 빨강은 ff가 가장 높은 값이기 때문이고 나머지는 가장낮은 값인 00으로 채워지기 때문이다.

### 예제

\#ff0000

\#0000ff

\#3cb371

\#ee82ee

\#ffa500

\#6a5acd



회색은 3가지의 색 원소를 갖게하면 된다.

### 예제

\#000000

\#3c3c3c

\#787878

\#b4b4b4

\#f0f0f0

\#ffffff

------

## HSL 값

HSL 색상은 hue, saturation, lightness 를합쳐서 HSL 이라는 형태를 사용한다

hsl(*hue*, *saturation*, *lightness*)

Hue는 0에서 360.0도 까지의 색상 바퀴이다. 0은 빨강 120은 초록 240은 파랑을 의미한다.

Saturation은 퍼센트 값을 의미하며 0%는 회색, 100%는 풀칼라를 의미한다.

Lightness또한 퍼센트값을 의미하며 0%는 검정 50%는 밝지도않고 어둡지도않은상태 100%는 흰색을 말한다

### 예제

hsl(0, 100%, 50%)

hsl(240, 100%, 50%)

hsl(147, 50%, 47%)

hsl(300, 76%, 72%)

hsl(39, 100%, 50%)

hsl(248, 53%, 58%)



------

### Saturation

Saturation은 색상의 강도로써 묘사될 수 있다.

100%는 순수한 색상이며 gray가 없는 색이다.

50%는 50%가 회색이며 여전히 색상을 볼 수 있는색이다.

0%는 완전희 회색이며 너는 더이상 이색상을 볼 수 없다

### 예제

hsl(0, 100%, 50%)

hsl(0, 80%, 50%)

hsl(0, 60%, 50%)

hsl(0, 40%, 50%)

hsl(0, 20%, 50%)

hsl(0, 0%, 50%)


[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_color_hsl_saturation)

------

### Lightness

색상의 빛은 색상에 얼마나 많은 빛을 주는지를 묘사한다. 0%는 black을 의미하며 50%는 반반 100%는 최고의 밝기(white)를 의미한다

### Example

hsl(0, 100%, 0%)

hsl(0, 100%, 25%)

hsl(0, 100%, 50%)

hsl(0, 100%, 75%)

hsl(0, 100%, 90%)

hsl(0, 100%, 100%)



------

회색은 hue와 saturation이 0으로 정의된다 

### 예제

hsl(0, 0%, 0%)

hsl(0, 0%, 24%)

hsl(0, 0%, 47%)

hsl(0, 0%, 71%)

hsl(0, 0%, 94%)

hsl(0, 0%, 100%)



------

## RGBA 값

RGBA 색상 값은 RGB색깔과 alpha 채널을 더한것이다. alpha 채널은 색상의 투명도를 말한다.

RGBA의 공식은 다음과 같다.

rgba(*red,* *green*, *blue, alpha*)

alpha 속성은 0은 완전 투명한 색이고 1은 불투명한 색이다.

### 예제

rgba(255, 99, 71, 0)

rgba(255, 99, 71, 0.2)

rgba(255, 99, 71, 0.4)

rgba(255, 99, 71, 0.6)

rgba(255, 99, 71, 0.8)

rgba(255, 99, 71, 1)



------

## HSLA 값

HSLA 색상값은 알파채널의 HSL 색상값의 확장이다.

HSLA의 공식은 다음과 같다.

hsla(*hue,* *saturation*, *lightness, alpha*)

alpha 속성은 0은 완전 투명한 색이고 1은 불투명한 색이다.

hsla(0, 100%, 50%, 0.5)

### 예제

hsla(9, 100%, 64%, 0)

hsla(9, 100%, 64%, 0.2)

hsla(9, 100%, 64%, 0.4)

hsla(9, 100%, 64%, 0.6)

hsla(9, 100%, 64%, 0.8)

hsla(9, 100%, 64%, 1)

[CSS Backgrounds](./CSS_backgrounds.md)

