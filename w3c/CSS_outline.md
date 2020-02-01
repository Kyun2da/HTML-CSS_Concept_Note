# CSS Outline

## CSS Outline

외곽선은 요소를 "눈에 띄게"만들기 위해 테두리 바깥에 요소 주위에 그려진 선이다.

CSS 다음과 같은 4가지의 속성을 갖는다.

- `outline-style`
- `outline-color`
- `outline-width`
- `outline-offset`
- `outline`

**Note:** 테두리와 outline선이 다르다! 테두리와 달리 outline선은 엘리먼트의 테두리 외부에 그려지며 다른 내용과 겹칠 수 있다. 또한 외곽선은 엘리먼트 치수의 일부가 아니다. 엘리먼트의 총 너비와 높이는 outline의 너비에 영향을받지 않는다.

------

## CSS Outline Style

 `outline-style` 속성은 outlinedml 스타일을 특화시키고 다음과 같은 값들중 하나의 값을 가질 수 있다.

- `dotted` - 점선
- `dashed` - 대쉬 선
- `solid` - 직선
- `double` - 이중 선
- `groove` - Defines a 3D grooved outline
- `ridge` - Defines a 3D ridged outline
- `inset` - Defines a 3D inset outline
- `outset` - Defines a 3D outset outline
- `none` - 아웃라인이 없음
- `hidden` - 아웃라인을 숨김

### Example

아웃라인 스타일을 설명한다.

```css
p.dotted {outline-style: dotted;}
p.dashed {outline-style: dashed;}
p.solid {outline-style: solid;}
p.double {outline-style: double;}
p.groove {outline-style: groove;}
p.ridge {outline-style: ridge;}
p.inset {outline-style: inset;}
p.outset {outline-style: outset;}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_outline-style)

**Note:** `outline-style` 속성이 설정되어 있지 않으면 다른 외곽선 속성 중 어느 것도 영향을 미치지 않습니다!

## CSS Outline Color

 `outline-color` 속성은 outline의 색을 조정할 수있다.

색은 다음속성에 의해 셋팅된다.

- name -  "red"와 같은 색 이름
- RGB - "rgb(255,0,0)"와 같은 RGB 값
- Hex -  "#ff0000"와 같은 hex값
- invert - 색상 반전을 수행한다 (색상 배경에 관계없이 윤곽선이 표시되도록 함)

다음 예는 색상이 다른 몇 가지 윤곽선을 보여준다. 또한이 요소들에는 윤곽선 안에 얇은 검은 색 테두리가 있다.

### 예제

```css
p.ex1 {
 border: 1px solid black;
 outline-style: solid;
 outline-color: red;
}

p.ex2 {
 border: 1px solid black;
 outline-style: double;
 outline-color: green;
}

p.ex3 {
 border: 1px solid black;
 outline-style: outset;
 outline-color: yellow;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_outline-color)

다음 예제는`outline-color : invert`를 사용하여 색상 반전을 수행한다. 이렇게하면 색상 배경에 관계없이 윤곽선이 표시된다.

### 예제

```css
p.ex1 {
 border: 1px solid yellow;
 outline-style: solid;
 outline-color: invert;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_outline-color_invert)

------

## CSS Outline Width

`outline-width` 속성은 아웃 라인의 너비를 지정하며 다음 값 중 하나를 가질 수 있다.

- thin (typically 1px)
- medium (typically 3px)
- thick (typically 5px)
- A specific size (in px, pt, cm, em, etc)

### 예제

```css
p.ex1 {
 border: 1px solid black;
 outline-style: solid;
 outline-color: red;
 outline-width: thin;
}

p.ex2 {
 border: 1px solid black;
 outline-style: solid;
 outline-color: red;
 outline-width: medium;
}

p.ex3 {
 border: 1px solid black;
 outline-style: solid;
 outline-color: red;
 outline-width: thick;
}

p.ex4 {
 border: 1px solid black;
 outline-style: solid;
 outline-color: red;
 outline-width: 4px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_outline-width)

------

## CSS Outline - Shorthand property

`outline` 속성은 다음과 같은 개별 개요 속성을 설정하기위한 속성이다.

- `outline-width`
- `outline-style` (required)
- `outline-color`

### 예제

```css
p.ex1 {outline: dashed;}
p.ex2 {outline: dotted red;}
p.ex3 {outline: 5px solid yellow;}
p.ex4 {outline: thick ridge pink;}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_outline)

------

## CSS Outline Offset

`outline-offset` 속성은 외곽선과 요소의 가장자리 / 테두리 사이에 공간을 추가한다. 요소와 윤곽선 사이의 공간은 투명하다.

### 예제

```css
p {
 margin: 30px;
 border: 1px solid black;
 outline: 1px solid red;
 outline-offset: 15px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_outline-offset)

### 예제

```css
p {
 margin: 30px;
 background: yellow;
 border: 1px solid black;
 outline: 1px solid red;
 outline-offset: 15px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_outline-offset2)

------

## All CSS Outline Properties

| 속성                                                         | 설명                                                         |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [outline](https://www.w3schools.com/cssref/pr_outline.asp)   | 한 번의 선언으로 외곽선 너비, 외곽선 스타일 및 외곽선 색상을 설정하는 속기 속성 |
| [outline-color](https://www.w3schools.com/cssref/pr_outline-color.asp) | 윤곽선의 색상을 설정                                         |
| [outline-offset](https://www.w3schools.com/cssref/css3_pr_outline-offset.asp) | 요소의 윤곽과 가장자리 또는 테두리 사이의 간격을 지정        |
| [outline-style](https://www.w3schools.com/cssref/pr_outline-style.asp) | 윤곽선의 스타일을 설정                                       |
| [outline-width](https://www.w3schools.com/cssref/pr_outline-width.asp) | 윤곽선의 너비를 설정                                         |