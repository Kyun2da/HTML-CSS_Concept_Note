# CSS Opacity / Transparency

`opacity` 속성은 엘리먼트의 투명도를 조절한다.

------

## Transparent Image

 `opacity` 속성은 0에서 1까지의 값을 가지고 값이 낮을 수록 더 투명해진다.

**Note:** IE8 이하에서는`filter : alpha (opacity = x)`를 사용한다. x는 0-100의 값을 가질 수 있습니다. 값이 낮을수록 요소가 더 투명 해진다.

### 예제

```css
img {
 opacity: 0.5;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_image_opacity)

------

## Transparent Hover Effect

`opacity`속성은 종종 `:hover`속성과 함께 사용된다 

### 예제

```css
img {
 opacity: 0.5;
}

img:hover {
 opacity: 1.0;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_image_transparency)

### Example explained

첫 번째 CSS 블록은 예제 1의 코드와 비슷하다. 또한 사용자가 이미지 중 하나를 가리킬 때 발생하는 동작을 추가했다. 이 경우 사용자가 이미지를 가리킬 때 이미지가 투명하지 않게만든다. 이를위한 CSS는`opacity : 1;`입니다.

마우스 포인터가 이미지에서 멀어지면 이미지가 다시 투명 해집니다.

호버 효과 반전의 예 :

### 예제

```css
img:hover {
 opacity: 0.5;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_image_transparency2)

------

## Transparent Box

'opacity'속성을 사용하여 요소의 배경에 투명성을 추가하면 모든 자식 요소가 동일한 투명성을 상속한다. 이렇게하면 완전히 투명한 요소 내부의 텍스트를 읽기 어렵게 만들 수 있다.

### 예제

```css
div {
 opacity: 0.3;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_opacity_box)

------

## Transparency using RGBA

위의 예와 같이 자식 요소에 불투명도를 적용하지 않으려면 **RGBA ** 색상 값을 사용하면된다.

[CSS 색상 장](https://www.w3schools.com/css/css_colors.asp)에서 RGB를 색상 값으로 사용할 수 있다는 것을 배웠다. RGB 외에도 알파 채널 (RGBA)과 함께 RGB 색상 값을 사용하여 색상의 불투명도를 지정할 수 있다.

### 예제

```css
div {
 background: rgba(76, 175, 80, 0.3) /* Green background with 30% opacity */
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_opacity_box2)

------

## Text in Transparent Box

### 예제

```html
<html>
<head>
<style>
div.background {
  background: url(klematis.jpg) repeat;
  border: 2px solid black;
}

div.transbox {
  margin: 30px;
  background-color: #ffffff;
  border: 1px solid black;
  opacity: 0.6;
}

div.transbox p {
  margin: 5%;
  font-weight: bold;
  color: #000000;
}
</style>
</head>
<body>

<div class="background">
  <div class="transbox">
    <p>This is some text that is placed in the transparent box.</p>
  </div>
</div>

</body>
</html>
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_transparency)

## 위의 예제 설명

먼저 배경 이미지와 테두리가있는 `<div>` 요소 (class = "background")를 만든다.

첫 번째 `<div>` 안에 다른 `<div>` (class = "transbox")를 만들 때.

`<div class = "transbox">`에는 배경색이 있고 테두리가 있다. div는 투명하다.


투명한 `<div>` 안에 `<p>` 요소 안에 텍스트를 추가한다.

[CSS Navigation Bar](./CSS_navigationbar.md)