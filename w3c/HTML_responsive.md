# HTML Responsive Web Design

![Responsive](https://www.w3schools.com/css/img_temp_band.jpg)

## 반응형 웹 디자인이란 무엇인가?

반응형 웹디자인은 HTML과 CSS를 자동적으로 크기, 숨기기, 줄이기, 크게하기, 웹사이트등을 재조정해주는 디자인을 말한다. 이것은 모든 기게에서 더 좋은 시각을 제공한다.

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_responsive_page)

**Note:** 웹페이지는 어느 기기에서나 보기 좋아야만 한다.

------

## 뷰포트를 세팅하기

반응형 웹 페이지를 만들 때 `<meta>`엘리먼트를 너의 웹페이지에 추가할 수 있다.

### 예제

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_responsive_viewport)

이것은 너의 웹페이지의 뷰포트를 셋팅하고 그것은 브라우저에게 어떻게 페이지의 크기오 ㅏ차원이 통제되어야 하는지를 줄 수 있다.

뷰포트 메타 태그가 없을 때 :
[![img](https://www.w3schools.com/css/img_viewport1.png)](https://www.w3schools.com/html/example_withoutviewport.htm)

뷰포트 메타 태그가 있을 때 :
[![img](https://www.w3schools.com/css/img_viewport2.png)](https://www.w3schools.com/html/example_withviewport.htm)

**Tip:** 만약 핸드폰이나 태블릿으로 이 페이지를 탐색한다면 너는 두개의 다른 차이를 볼 수 있을 것이다.

------

## 반응형 이미지

반응형 이미지는 어떠한 브라우저 사이즈에서도 나이스한 스케일로 적용된다

### Using the width Property

만약 CSS 넓이 속성을 100%로 적용하면 이미지는 반응적으로 스케일을 크게하거나 줄일 것이다.

![img](https://www.w3schools.com/html/img_girl.jpg)

### 예제

```html
<img src="img_girl.jpg" style="width:100%;">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_responsive_image)

위의 예제에서 이미지는 그것의 오리지널 사이즈보다 커질 수 있다. 더 나은 해결책은 max-width속성을 대신 사용하는 것이다

### Using the max-width Property

만약 `max-width` 속성을 100%로 세팅한다면 이미지는 그것이 필요하다면 축소는 되지만 그것의 오리지널 사이즈보다는 커지지는 않을 것이다.

![img](https://www.w3schools.com/html/img_girl.jpg)

### 예제

```html
<img src="img_girl.jpg" style="max-width:100%;height:auto;">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_responsive_image_maxwidth)

------

### 브라우저의 넓이에 따라 다른 이미지를 보여주기

HTML `<picture>`엘리먼트는 너에게 브라우저 윈도우 크기에 따라서 다른 이미지를 보여줄수 있게 할 수 있다.

브라우저 윈도우의 크기를 줄이거나 늘리면 넓이에 따라 이미지가 바뀌는 것을 볼 수 있다.

![Flowers](https://www.w3schools.com/html/img_smallflower.jpg)



### 예제

```html
<picture>
 <source srcset="img_smallflower.jpg" media="(max-width: 600px)">
 <source srcset="img_flowers.jpg" media="(max-width: 1500px)">
 <source srcset="flowers.jpg">
 <img src="img_smallflower.jpg" alt="Flowers">
</picture>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_responsive_picture)

------

## 반응형 텍스트 사이즈

텍스트 사이즈는 "vw" 단위로 세팅될 수 있는데 이것은 "viewport width"를 의미한다.

브라우저 윈도우의 크기를 텍스트 사이즈에 맞게하는 방법이다.

### 예제

```css
<h1 style="**font-size:10vw**">Hello World</h1>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_responsive_text)

뷰포트는 브라우저 윈도우 사이즈이다. 1vw = 1%의 뷰포트 넓이다. 만약 뷰포트가 50cm의 넓이라면 1vw는 0.5cm를 의미한다.

------

## 미디어 쿼리

텍스트나 이미지의 크기를 재조정하는 것은 반응형 웹페이지에서 미디어 쿼리를 사용하는 일은 일반적이다. 미디어 쿼리에서 너는 완전하게 다른 브라우저 사이즈를 위하여 다른 스타일들을 정의할 수 있다.

### 예제

```css
<style>
.left, .right {
  float: left;
  width: 20%; /* The width is 20%, by default */
}

.main {
  float: left;
  width: 60%; /* The width is 60%, by default */
}

/* Use a media query to add a breakpoint at 800px: */
@media screen and (max-width: 800px) {
  .left, .main, .right {
    width: 100%; /* The width is 100%, when the viewport is 800px or smaller */
  }
}
</style>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_responsive_media_query)

**Tip:** 미디어쿼리와 반응형 웹페이지를 배우기 위해서 오른쪽의 링크를 읽어봐라 [RWD Tutorial](https://www.w3schools.com/css/css_rwd_intro.asp).

------

## 반응형 웹페이지 - Full Example

반응형 웹페이지는 큰 데스크톱 화면과 작은 모바일 폰에서 좋아 보여야 한다.

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_responsive_media_query3)

------

## 반응형 웹디자인 - Frameworks

반응형 웹디자인을 공급하는 많은 CSS프레임워크들이 있다.

그것들은 사용하기 쉽고 공짜이다.

##  W3.CSS 사용하기

반응형 웹디자인을 만드는 좋은 방법중 하나는 반응형 스타일시트를 사용하는 것이다.[W3.CSS](https://www.w3schools.com/w3css/default.asp) 같은..

W3.CSS는 그것을 어떠한 사이즈에서도 더 나이스한 시각효과를 제공한다.

### 예제

```html
<!DOCTYPE html>
<html>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<body>

<div class="w3-container w3-green">
  <h1>W3Schools Demo</h1>
  <p>Resize this responsive page!</p>
</div>

<div class="w3-row-padding">
  <div class="w3-third">
    <h2>London</h2>
    <p>London is the capital city of England.</p>
    <p>It is the most populous city in the United Kingdom,
    with a metropolitan area of over 13 million inhabitants.</p>
  </div>

  <div class="w3-third">
    <h2>Paris</h2>
    <p>Paris is the capital of France.</p>
    <p>The Paris area is one of the largest population centers in Europe,
    with more than 12 million inhabitants.</p>
  </div>

  <div class="w3-third">
    <h2>Tokyo</h2>
    <p>Tokyo is the capital of Japan.</p>
    <p>It is the center of the Greater Tokyo Area,
    and the most populous metropolitan area in the world.</p>
  </div>
</div>

</body>
</html>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_responsive_w3css)

W3.CSS에 대해 배우려면 오른쪽의 링크를 참조하라 [W3.CSS Tutorial](https://www.w3schools.com/w3css/default.asp).

------

## 부트스트랩

또다른 인기있는 프레임워크로는 부트스트랩이 있다. 이것은 반응형 웹페이지를 만들기 위해 HTML, CSS, jQuery를 사용한다.

### 예제

```html
<!DOCTYPE html>
<html lang="en">
<head>
<title>Bootstrap Example</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.0/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
</head>
<body>

<div class="container">
  <div class="jumbotron">
    <h1>My First Bootstrap Page</h1>
  </div>
  <div class="row">
    <div class="col-sm-4">
      ...
    </div>
    <div class="col-sm-4">
      ...
    </div>
    <div class="col-sm-4">
    ...
    </div>
  </div>
</div>

</body>
</html>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_responsive_bootstrap)

부트스트랩에 대해 배우려면 오른쪽의 링크를 참조하라 [Bootstrap Tutorial](https://www.w3schools.com/bootstrap/default.asp).

[HTML Computer Code Elements](./HTML_computercode.md)