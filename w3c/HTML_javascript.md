# HTML JavaScript

javascript는 HTML 페이지를 더 동적이고 활동적이게 만든다.

------

## The HTML `<script>` Tag

`<script>`태그는 client-side 스크립트로 정의되곤 한다.

`<script>`엘리먼트는 스크립트 상태를 포함하거나 그것은 `src`속성을 통하여 외부 스크립트 파일을 가리킨다.

### 예제

```html
<script>
    document.getElementById("demo").innerHTML = "Hello JavaScript!";</script>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_script)

**Tip:** 너는 우리의 [JavaScript Tutorial](https://www.w3schools.com/js/default.asp)을 통해서 자바스크립트를 더 배울 수 있다.

------

## A Taste of JavaScript

여기에 자바스크립트로 할 수 있는 몇몇 예제가 있다.

### 자바스크립트는 HTML내용을 변화 시킬 수있다.

```javascript
document.getElementById("demo").innerHTML = "Hello JavaScript!";
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_script_html)

### 자바스크립트는 HTML style을 변화시킬 수 있다.

```javascript
document.getElementById("demo").style.fontSize = "25px";
document.getElementById("demo").style.color = "red";
document.getElementById("demo").style.backgroundColor = "yellow";
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_script_styles)

### 자바스크립트는 HTML속성을 변화시킬 수 있다.

```javascript
document.getElementById("image").src = "picture.gif";
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_script_attribute)

------

## The HTML `<noscript>` Tag

`<noscript>`태그는 자바스크립트를 서포팅하지 않는 유저의 브라우저에서 그들의 대신에 불가능하다는것을 보여줄 때 대안적인 스크립트 태그이다.

### Example

```javascript
<script>
    document.getElementById("demo").innerHTML = "Hello JavaScript!";</script>
<noscript>Sorry, your browser does not support JavaScript!</noscript>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_noscript)

------

## HTML Script Tags

| 태그         | 설명                                                         |
| :----------- | :----------------------------------------------------------- |
| `<script>`   | client-side 스크립트를 정의한다.                             |
| `<noscript>` | client-side스크립트를 지원하지 않는 유저에게 대체 내용을 보여준다. |

------

[HTML File Paths](./HTML_filepath.md)



