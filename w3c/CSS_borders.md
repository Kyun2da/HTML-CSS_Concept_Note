# CSS Borders

## CSS 테두리 속성

CSS `border` 속성은 너에게 테두리의 색, 넓이, 스타일을 제공해준다



------

## CSS Border Style

 `border-style` 속성은 어떤 속성의 종류를 보여줄지 특화시킨다.

아래는 그에 대한 속성값이다.

- `dotted` - 점선테두리
- `dashed` - 대쉬 테두리
- `solid` - 굵은 테두리
- `double` - 이중 테두리
- `groove` - 3D테두리. 이효과는 테두리 색상값에 달려있다.
- `ridge` - ridge테두리. 이효과는 테두리 색상값에 달려있다.
- `inset` - 3D inset테두리. 이효과는 테두리 색상값에 달려있다.
- `outset` - 3D outset테두리. 이효과는 테두리 색상값에 달려있다.
- `none` - 테두리 없음
- `hidden` - 숨어있는 테두리

 `border-style` 속성은 1~4가지 값을 가질 수 있다. (top, right, bottom, left)

### 예제

```css
p.dotted {border-style: dotted;}
p.dashed {border-style: dashed;}
p.solid {border-style: solid;}
p.double {border-style: double;}
p.groove {border-style: groove;}
p.ridge {border-style: ridge;}
p.inset {border-style: inset;}
p.outset {border-style: outset;}
p.none {border-style: none;}
p.hidden {border-style: hidden;}
p.mix {border-style: dotted dashed solid double;}
```



[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_border-style)

**Note:** border-style 속성이 설정되어 있지 않으면 아래에 설명 된 OTHER CSS 테두리 속성 중 어느 것도 영향을 미치지 않는다.

------

## CSS 테두리 넓이

`border-width`속성은 네가지 테두리의 넓이를 다룬다.

넓이는 특수한 사이즈(px, pt, cm, em, etc)에 의해 정의된다. 얇거나 중간이거나 굵은 값으로

`border-width`속성은 1~4가지 값을 가져올 수 있다.(왼쪽 오른쪽 위 아래)

### 예제

```css
p.one {
 border-style: solid;
 border-width: 5px;
}

p.two {
 border-style: solid;
 border-width: medium;
}

p.three {
 border-style: solid;
 border-width: 2px 10px 4px 20px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_border-width)

------

## CSS Border Color

`border-color`속성은 네가지의 테두리의 색상을 다루는데 사용된다.

- name - "red"와 같은 이름을 사용한다
- Hex - "#ff0000"와 같은 값을 사용한다
- RGB - "rgb(255,0,0)"와 같은 값을 사용한다.
- transparent

 `border-color` 속성은 1~4가지의 값을 사용한다.

 `border-color`값이 셋팅되지 않으면 이것은 엘리먼트의 색을 상속한다.

### 예제

```css
p.one {
 border-style: solid;
 border-color: red;
}

p.two {
 border-style: solid;
 border-color: green;
}

p.three {
 border-style: solid;
 border-color: red green blue yellow;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_border-color1)

------

## CSS Border - Individual Sides

이 예로부터 너는 각각의 면의 다른 테두리 속성이 가능하다는 것을 볼 수 있다.

또한 CSS에서도 각각의 테두리 스타일을 정의하다는 것이 가능하다는 것이다.

### 예제

```css
p {
 border-top-style: dotted;
 border-right-style: solid;
 border-bottom-style: dotted;
 border-left-style: solid;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_border-side)

### 예제

```css
p {
 border-style: dotted solid;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_border-side2)

그래서 다음과 같이 동작한다.

만약 `border-style` 속성이 네가지 값을 가지면

- border-style: dotted solid double dashed; (위에서부터 시계방향)
  - 맨위는 dotted
  - 오른쪽은 solid
  - 아래는 double
  - 왼쪽은 dashed이다

만약 `border-style` 속성이 세가지 값을 가지면

- border-style: dotted solid double; (시계방향)
  - 위는 dotted
  - 오른쪽은 solid
  - 아래는 double

만약 `border-style` 속성이 두가지 값을 가지면

- border-style: dotted solid;
  - 위와 아래는 dotted
  - 왼쪽과 오른쪽은 solid

만약 `border-style` 속성이 한가지 값을 가지면

- border-style: dotted;
  - 네개의 테두리는 모두 dotted이다

`border-style`속성은 위의 예에서 사용된다. 그러나 border-width와 border-color또한 위와 같이 동작한다

------

## CSS Border - Shorthand Property

너도 알다시피 위의 예제처럼 많은 테두리를 다루는 속성들이 있다.

코드를 짧게 하기 위해 각각의 테두리 속성을 하나의 속성으로 압축하는 것이 가능하다.

`border`속성은 개인적인 테두리 짧은 속성이 가능하다.

- `border-width`
- `border-style` (required)
- `border-color`

### 예제

```css
p {
 border: 5px solid red;
}
```



### Left Border

```css
p {
 border-left: 6px solid red;
 background-color: lightgrey;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_border_left)

### Bottom Border

```css
p {
 border-bottom: 6px solid red;
 background-color: lightgrey;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_border_bottom)

------

## CSS Rounded Borders

The `border-radius` 속성은 엘리먼트에 둥근 테두리를 적용하는데 사용된다.

### 예제

```css
p {
 border: 2px solid red;
 border-radius: 5px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_border_round)

**Note:**  `border-radius` 속성은 IE8과 더 이른 버전에서 호환되지 않는다.



------

## 모든 CSS 테두리 속성

| Property                                                     | Description                                            |
| :----------------------------------------------------------- | :----------------------------------------------------- |
| [border](https://www.w3schools.com/cssref/pr_border.asp)     | 모든 테두리 속성을 하나의 선언으로 처리한다            |
| [border-bottom](https://www.w3schools.com/cssref/pr_border-bottom.asp) | 테두리 아랫쪽을 처리한다                               |
| [border-bottom-color](https://www.w3schools.com/cssref/pr_border-bottom_color.asp) | 테두리 아래 색깔을 처리한다                            |
| [border-bottom-style](https://www.w3schools.com/cssref/pr_border-bottom_style.asp) | 테두리 아래 스타일을 처리한다                          |
| [border-bottom-width](https://www.w3schools.com/cssref/pr_border-bottom_width.asp) | 테두리 아래 넓이를 처리한다                            |
| [border-color](https://www.w3schools.com/cssref/pr_border-color.asp) | 네개의 테두리의 색상을 정의한다.                       |
| [border-left](https://www.w3schools.com/cssref/pr_border-left.asp) | Sets all the left border properties in one declaration |
| [border-left-color](https://www.w3schools.com/cssref/pr_border-left_color.asp) | 테두리 왼쪽의 색상을 정의한다.                         |
| [border-left-style](https://www.w3schools.com/cssref/pr_border-left_style.asp) | 테두리 왼쪽의 스타일을 정의한다.                       |
| [border-left-width](https://www.w3schools.com/cssref/pr_border-left_width.asp) | 테두리 왼쪽의 넓이를 정의한다.                         |
| [border-radius](https://www.w3schools.com/cssref/css3_pr_border-radius.asp) | 테두리의 둥근 모서리를 정의한다.                       |
| [border-right](https://www.w3schools.com/cssref/pr_border-right.asp) | 테두리의 오른쪽을 정의한다.                            |
| [border-right-color](https://www.w3schools.com/cssref/pr_border-right_color.asp) | 테두리의 오른쪽 색상을 정의한다.                       |
| [border-right-style](https://www.w3schools.com/cssref/pr_border-right_style.asp) | 테두리의 오른쪽 스타일을 정의한다.                     |
| [border-right-width](https://www.w3schools.com/cssref/pr_border-right_width.asp) | 테두리의 오른쪽 넓이를 정의한다.                       |
| [border-style](https://www.w3schools.com/cssref/pr_border-style.asp) | 테두리 스타일을 정의한다.                              |
| [border-top](https://www.w3schools.com/cssref/pr_border-top.asp) | 테두리의 윗쪽 속성을 정의한다.                         |
| [border-top-color](https://www.w3schools.com/cssref/pr_border-top_color.asp) | 테두리의 윗쪽 색상을 정의한다.                         |
| [border-top-style](https://www.w3schools.com/cssref/pr_border-top_style.asp) | 테두리의 윗쪽 스타일을 정의한다.                       |
| [border-top-width](https://www.w3schools.com/cssref/pr_border-top_width.asp) | 테두리의 윗쪽 넓이를 정의한다.                         |
| [border-width](https://www.w3schools.com/cssref/pr_border-width.asp) | 테두리의 넓이를 정의한다.                              |

[CSS Margins](./CSS_margins.md)

