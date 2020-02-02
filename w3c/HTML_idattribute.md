# HTML The id Attribute

## Using The id Attribute

`id` 속성은 하나의 HTML 엘리먼트를 위한 단일의 id를 정의하는데에 특화되어 있다.

id값은 CSS와 Javascript에의해 사용될 수 있고 특수한 id 값을 가진 엘리먼트로 특정한 task를 수행한다.

### 예제

id "myHeader"를 사용해서 엘리먼트에 css스타일을 사용하기

```html
<style>
#myHeader {
  background-color: lightblue;
  color: black;
  padding: 40px;
  text-align: center;
}
</style>

<h1 id="myHeader">My Header</h1>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_id_css)

**Tip:** 어떠한 HTML엘리먼트던지 id 속성을 사용할 수 있다.

**Note:** id 값은 어떨경우에는 민감하다

**Note:** id 값은 항상 적어도 하나의 문자를 포함해야하고 공백은 들어가서는 안된다

------

## Difference Between Class and ID

HTML엘리먼트는 하나의 유니크한 아이디 값을 가질 수 있고 하나의 엘리먼트에만 결속된다. 반면 클래스 이름은 다중의 엘리먼트에 의해 사용될 수 있다.

### 예제

```html
<style>
/* Style the element with the id "myHeader" */
#myHeader {
  background-color: lightblue;
  color: black;
  padding: 40px;
  text-align: center;
}

/* Style all elements with the class name "city" */
.city {
  background-color: tomato;
  color: white;
  padding: 10px;
}
</style>

<!-- A unique element -->
<h1 id="myHeader">My Cities</h1>

<!-- Multiple similar elements -->
<h2 class="city">London</h2>
<p>London is the capital of England.</p>

<h2 class="city">Paris</h2>
<p>Paris is the capital of France.</p>

<h2 class="city">Tokyo</h2>
<p>Tokyo is the capital of Japan.</p>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_id_class)

**Tip:** css튜토리얼에서 더많은 것들을 배울 수 있다 [CSS Tutorial](https://www.w3schools.com/css/default.asp).

## Bookmarks with ID and Links

HTML 북마크들은 독자가 웹페이지의 특정한 부분으로 점프할 수 있도록 도와준다

북마크는 만약 웹페이지가 매우 길다면 아주 유용하다.

북마크를 만들기 위하여 너는 처음에 북마크를 만들어야만하고 그것에 대해 링크를 걸어야한다.

링크가 클릭되면, 페이지는 북마크 위치로 스크롤될 것이다.

## 예제

처음에 id속성을 북마크로 만든다.

```html
<h2 id="C4">Chapter 4</h2>
```

그후에 같은 페이지 이내에 있는 북마크에 링크를 추가한다.

```html
<a href="#C4">Jump to Chapter 4</a>
```

또는 다른 페이지에 북마크를 추가한다.

### 예제

```html
<a href="html_demo.html#C4">Jump to Chapter 4</a>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_links_bookmark)

------

## Using The id Attribute in JavaScript

자바스크립트는 `getElementBtId()`메소드를 통해서 id에 접근할 수있다.

### 예제

자바스크립트를통하여 id속성에 접근하기

```javascript
<script>
function displayResult(){  
	document.getElementById("myHeader").innerHTML = "Have a nice day!";
}
</script>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_id_js)

[HTML iframes](./HTML_iframes.md)



