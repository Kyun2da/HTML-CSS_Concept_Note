# CSS Layout - Horizontal & Vertical Align

## Center Align Elements

블록 엘리먼트를 중앙으로 정렬하기 위해서는 `margin: auto`를 사용해야 한다.

엘리먼트의 넓이를 세팅하는것은 그것의 컨테이너의 가장자리로 늘어나지 않는다.

그렇게 하면 엘리먼트가 지정된 너비를 차지하고 나머지 공간은 두 여백을 동일하게 나누게 된다.

### 예제

```css
.center {
 margin: auto;
 width: 50%;
 border: 3px solid green;
 padding: 10px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_align_container)

**Note:** `width`속성이 설정되어 있지 않거나 100%로 설정되어 있으면 중앙 정렬이 적용되지 않는다.

------

## Center Align Text

텍스트 안에 엘리먼트를 중앙에 위치시키려면 `text-align : center`를 사용해야 한다.

### 예제

.center {
 text-align: center;
 border: 3px solid green;
}

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_align_text)

**Tip:** 텍스트를 정렬하는 방법에 대한 자세한 예는 [CSS 텍스트](https://www.w3schools.com/css/css_text.asp) 장을 참조.

------

## Center an Image

이미지를 중앙에 맞추려면 왼쪽 및 오른쪽 여백을`auto`로 설정하고`block` 요소로 만든다.

### 예제

```css
img {
 display: block;
 margin-left: auto;
 margin-right: auto;
 width: 40%;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_align_image)

------

## Left and Right Align - Using position

요소를 정렬하는 한 가지 방법은`position : absolute;`를 사용하는 것이다.

### 예제

```css
.right {
 position: absolute;
 right: 0px;
 width: 300px;
 border: 3px solid #73AD21;
 padding: 10px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_align_pos)

**Note:** 절대 위치 요소는 정상 흐름에서 제거되며 요소와 겹칠 수 있다.

------

## Left and Right Align - Using float

요소를 정렬하는 또 다른 방법은`float` 속성을 사용하는 것이다.

### 예제

```css
.right {
 float: right;
 width: 300px;
 border: 3px solid #73AD21;
 padding: 10px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_align_float)

**Note:** 요소가 포함 된 요소보다 키가 크고 부동 상태 인 경우 컨테이너 외부로 오버플로됩니다. "**clearfix **"핵을 사용하여이 문제를 해결할 수 있다 (아래 예 참조).

------

## The clearfix Hack

### Without Clearfix

![img](https://www.w3schools.com/howto/clearfix_prob.jpg)

### With Clearfix

![img](https://www.w3schools.com/howto/clearfix_solution.jpg)

그런 다음 포함 요소에`overflow : auto;`를 추가하여이 문제를 해결할 수 있다.

### 예제

```css
.clearfix {
 overflow: auto;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_clearfix)

------

## Center Vertically - Using padding

CSS에서 요소를 세로로 가운데 맞추는 방법에는 여러 가지가 있다. 간단한 해결책은 상단 및 하단 '패딩'을 사용하는 것이다.

### 예제

```css
.center {
 padding: 70px 0;
 border: 3px solid green;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_align_padding)

세로 및 가로로 가운데에 맞추려면`padding` 및`text-align : center`를 사용하면된다.

### 예제

```css
.center {
 padding: 70px 0;
 border: 3px solid green;
 text-align: center;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_align_padding2)

------

## Center Vertically - Using line-height

또 다른 방법은`line-height` 속성을`height` 속성과 같은 값으로 사용하는 것이다.

### 예제

```css
.center {
 line-height: 200px;
 height: 200px;
 border: 3px solid green;
 text-align: center;
}

/* If the text has multiple lines, add the following: */
.center p {
 line-height: 1.5;
 display: inline-block;
 vertical-align: middle;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_align_line-height)

------

## Center Vertically - Using position & transform

`padding`과  `line height`가  옵션이 아닌 경우 세 번째 해결책은 위치 지정과  `transform` 속성을 사용하는 것이다.

### 예제

```css
.center {
 height: 200px;
 position: relative;
 border: 3px solid green;
}

.center p {
 margin: 0;
 position: absolute;
 top: 50%;
 left: 50%;
 transform: translate(-50%, -50%);
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_align_transform)

**Tip:** [2D Transforms Chapter](https://www.w3schools.com/css/css3_2dtransforms.asp)에서 변형 속성에 대해 자세히 알아 본다.

[CSS Combinators](./CSS_combinators.md)