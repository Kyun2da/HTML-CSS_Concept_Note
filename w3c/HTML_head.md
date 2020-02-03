# HTML Head

## The HTML `<head>` Element

이 `<head>`엘리먼트는 메타데이터를 위한 컨테이너이고 `<html>`태그와 `<body>`태그 사이에 위치되어 있다.

HTML 메타데이터는 HTML 문서에 관한 데이터이다. 메타데이터는 보여지지 않는다.

메타데이터는 전형적으로 문서 제목, 문자 셋팅, 스타일, 스크립트 그리고 다른 메타 정보로 이루어 진다.

이러한 태그를 메타데이터는 묘사한다 : `<title>`, `<style>`, `<link>`, `<script>`, `<base>`

## The HTML <title> Element

`<title>`엘리먼트는 문서의 제목을 정의한다. 그리고 모든 HTML 문서에서 요구된다.

`<title>`엘리먼트

- 브라우저 탭에서 보이는 제목을 의미
- 즐겨찾기에 추가될 때 페이지를 위한 제목을 공급한다.
- 검색엔진 결과에서 페이지를 위한 제목을 보여준다.

간단한 HTML 문서 예제

### 예제

```html
<!DOCTYPE html>
<html>

<head>
 <title>Page Title</title>
</head>

<body>
The content of the document......
</body>

</html>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_head_title)

------

## The HTML `<style>` Element

`<style>`엘리먼트는 하나의 간단한 HTML페이지를 위해 스타일 정보를 정의하기 위해 사용된다.

### 예제

```html
<style>  
    body {background-color: powderblue;}  
    h1 {color: red;}  
    p {color: blue;}
</style>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_head_style)

------

## The HTML `<link>` Element

`<link>`엘리먼트는 외부 스타일시트를 가져오기 위해서 링크를 사용하기 위한 엘리먼트다.

### 예제

```html
<link rel="stylesheet" href="mystyle.css">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_head_link)

**Tip:** CSS에관해 배우고 싶으면 이곳을 참조해라  [CSS Tutorial](https://www.w3schools.com/css/default.asp).

------

## The HTML `<meta>` Element

`<meta>`엘리먼트는 문자 셋팅, 페이지 설명, 키워드, 작가, 다른 메타데이터들의 설명을 위해 사용된다.

메타데이터는 브라우저에 의해 사용되고, 검색 엔진에의해 사용되고, 또다른 여러 웹서비스에 의해 사용된다.

문자셋팅을 사용하는 것은 다음과 같다.

```html
<meta charset="UTF-8">
```

웹페이지의 설명을 하는 것은 다음과 같다.

```html
<meta name="description" content="Free Web tutorials">
```

검색엔진의 키워드를 정의하는 것은 다음과 같다.

```html
<meta name="keywords" content="HTML, CSS, XML, JavaScript">
```

페이지의 작가를 정의하는 것은 다음과 같다.

```html
<meta name="author" content="John Doe">
```

매 30초마다 문서를 갱신하는 것은 다음과 같다.

```html
<meta http-equiv="refresh" content="30">
```

다음은 `<meta>`태그의 예제이다.

### 예제

```html
<meta charset="UTF-8">
<meta name="description" content="Free Web tutorials"><meta name="keywords" content="HTML,CSS,XML,JavaScript">
<meta name="author" content="John Doe">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_head_meta)

------

## Setting The Viewport

HTML5는 웹디자이너에게   `<meta>` 태그를 통해  뷰포트를 통제하는방법을 알려준다.

뷰포트는 웹페이지의 유저의 볼 수있는 영역이라는 뜻이다. 이것은 기기들에 따라 다양하며 모바일에서는 더작을 수 있고 컴퓨터 스크린에서는 더 클 수 잇다.

너는 모든 너의 웹페이지안에 `<meta>`뷰포트 엘리먼트를 포함해야만 한다.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

 `<meta>` 뷰포트 엘리먼트는 브라우저에게 어떻게 페이지의 차원이나 크기를 통제하는 지를 알려준다.

width=device-with 부분은 기기의 스크린의 넓이에 따라서 페이지의 넓이를 지정하게 해준다.

initial-scale=1.0 부분은 브라우저에 의해 처음 페이지가 로드 될 때 줌 수준을 지정해 주는 것이다

여기에 페이지의 뷰포트 메타 태그 없이 쓴예제와 뷰포트 메타태그를 쓴 예제가 있다

**Tip:** 만약 너가 핸드폰이나 타블릿으로 이페이지를 열면 너는 두개의 차이점을 볼 수 있을 것이다.

![img](https://www.w3schools.com/css/img_viewport1.png)

**Without the viewport meta tag**](https://www.w3schools.com/html/example_withoutviewport.htm)



![img](https://www.w3schools.com/css/img_viewport2.png)

**With the viewport meta tag**](https://www.w3schools.com/html/example_withviewport.htm)



------

## The HTML `<script>` Element

`<script>`엘리먼트는 고객중심의 자바스크립트를 정의하는데 사용된다.

자바스크립트는 HTML 엘리먼트의 id=demo를 가진것에 Hello JavaScript라고 쓸 수 있다.

### 예제

```javascript
<script>
   function myFunction{
       document.getElementById("demo").innerHTML = "HelloJavaScript!";
   }
</script>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_head_script)

**Tip:** 자바스크립트에 대해 더 배우고 싶다면 이곳을 참조해라 [JavaScript Tutorial](https://www.w3schools.com/js/default.asp).

------

## The HTML `<base>` Element

`<base>`는 페이지의 모든 상대 URL에 대한 기본 URL 및 기본 대상을 지정한다.

### 예제

```html
<base href="https://www.w3schools.com/images/" target="_blank">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_head_base)

------

## Omitting `<html>`, `<head>` and `<body>`?

HTML5 표준에 의하면 `<html>` ,  `<body>` , `<head>` 태그는 생략할 수있다.

### 예제

```css
<!DOCTYPE html>
<title>Page Title</title>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_head_none)

**Note:**

W3School은 이러한 `<html>`태그와 `<body>`태그를 생략하는 것을 추천하지 않는다. 이러한 태그를 생략하면 DOM이나 XML 소프트웨어에 충돌을 일으킬 수있고 IE9와 같은 다른 브라우저에서 에러를 일으킬 수 있다.

그러나 `<head>`태그를 생략하는 것은 오랫동안 일반적인 관행이 되곤 했다.

------

## HTML head Elements

| 태그       | 설명                                                  |
| :--------- | :---------------------------------------------------- |
| `<head>`   | 문서에 관해 정보를 정의한다.                          |
| `<title>`  | 문서의 제목을 정의한다.                               |
| `<base>`   | 페이지의 링크에 기본 타겟값이나 기본 주소를 정의한다. |
| `<link>`   | 외부 소스와 문서사이에  관계를 정의한다.              |
| `<meta>`   | HTML 문서에 관해 메타데이터를 정의한다.               |
| `<script>` | 클라이언트측의 스크립트를 정의한다.                   |
| `<style>`  | 문서를 위한 스타일 정보를 정의한다.                   |

[HTML Layout](./HTML_layout.md)

