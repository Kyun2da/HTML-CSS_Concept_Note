# HTML The class Attribute

## Class 속성을 사용하기

HTML `class` 속성은 같은 클래스 이름의 엘리먼트들을 같은 스타일을 적용할 때 사용한다.

그래서 같은  `class` 속성을 갖고있는 모든 HTML 엘리먼트 는 같은 스타일을 가질 것이다.

여기에 우리가 3개의`<div>` 엘리먼트를 같은 클래스 이름으로 한 예시이다.

### 예제

```html
<!DOCTYPE html>
<html>
<head>
<style>
.cities {
  background-color: black;
  color: white;
  margin: 20px;
  padding: 20px;
}
</style>
</head>
<body>

<div class="cities">
  <h2>London</h2>
  <p>London is the capital of England.</p>
</div>

<div class="cities">
  <h2>Paris</h2>
  <p>Paris is the capital of France.</p>
</div>

<div class="cities">
  <h2>Tokyo</h2>
  <p>Tokyo is the capital of Japan.</p>
</div>

</body>
</html>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_classes_capitals)



## Using The class Attribute on Inline Elements

HTML `class` 속성은 inline 엘리먼트에서도 사용될 수 있다.

### 예제

```html
<!DOCTYPE html>
<html>
<head>
<style>
span.note {
  font-size: 120%;
  color: red;
}
</style>
</head>
<body>

<h1>My <span class="note">Important</span> Heading</h1>
<p>This is some <span class="note">important</span> text.</p>

</body>
</html>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_classes_span)

**Tip:**  `class` 속성은 어떠한 HTML 엘리먼트에서든지 사용될 수 있다.

**Note:** 클래스 이름은 매우 예민하다

**Tip:** 우리의 [CSS Tutorial](https://www.w3schools.com/css/default.asp)에서 더많은 CSS 예제들에 대해 배워보자.

------

## Select Elements With a Specific Class

CSS에서 특수한 클래스를 가진 엘리먼트를 선택하기 위해서는 . 문자를 쓴 후 다음에 클래스의 이름이 오도록 한다.

### 예제

CSS스타일을 city이름의 클래스르 쓰고있는 모든 엘리먼트에 사용하라

```html
<style>
.city {
  background-color: tomato;
  color: white;
  padding: 10px;
}
</style>

<h2 class="city">London</h2>
<p>London is the capital of England.</p>

<h2 class="city">Paris</h2>
<p>Paris is the capital of France.</p>

<h2 class="city">Tokyo</h2>
<p>Tokyo is the capital of Japan.</p>
```



[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_classes_css)

------

## Multiple Classes

HTML 엘리먼트는 하나의 클래스 이름보다 더많은 클래스를 가질수 있고 각각의 클래스는 공간에 의해 분리되야만 한다.

### 예제

이 예제에서 하나의 엘리먼트와 main, city라는 두개의 클래스를 갖는 예제이다.

```html
<h2 class="city main">London</h2>
<h2 class="city">Paris</h2>
<h2 class="city">Tokyo</h2>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_classes_multiple)

위의 예제에서 첫번째 `<h2>`엘리먼트는 city와 main클래스 두개에 결속된다.

------

## Different Tags Can Share Same Class

`<h2>`와 `<p>`태그와 같이 다른태그들도 같은 클래스 이름을 가질 수 있고 그 스타일 또한 공유된다.

### 예제

```html
<h2 class="city">Paris</h2>
<p class="city">Paris is the capital of France</p>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_classes_tags)

------

## Using The class Attribute in JavaScript

자바스크립트에서도 특수한 클래스의 이름을 가진 엘리먼트를 선택할 수 있다.

자바스크립트는 `getElementsByClassName()`메소드를 사용해 클래스에 접근할 수 있다.

### 예제

유저가 버튼을 클릭하면 city이름을 가진 모든 엘리먼트가 숨겨진다.

```javascript
<script>
function myFunction() {
  var x = document.getElementsByClassName("city");
  for (var i = 0; i < x.length; i++) {
    x[i].style.display = "none";
  }
}
</script>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_classes_js)

위의 코드 예제에서 너가 이해를 못했더라도 걱정하지 마라

너는 우리의 자바스크립트 챕터에서 더 배울 수 있고[HTML JavaScript](https://www.w3schools.com/html/html_scripts.asp) 자바스크립트 튜토리얼에서도 배울 수 있다[JavaScript Tutorial](https://www.w3schools.com/js/default.asp).

[HTML id](./HTML_idattribute.md)