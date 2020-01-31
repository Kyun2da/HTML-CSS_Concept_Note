# HTML Block and Inline Elements



모든 HTML 엘리먼트는 요소 유형에 따라 기본 표시값이 있다.

두 표시값은 블록과 인라인이다.

------

## Block-level Elements

블록-수준 엘리먼트는 항상 새줄에서 시작하여 사용 가능한 전체 너비를 차지한다.

대표적인 엘리먼트로 div가 있다.

### 예제

```html
<div>Hello World</div>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_block_div)

HTMl에는 다음과 같은 블록-수준 엘리먼트들이 있다.

- `<address>`
- `<article>`
- `<aside>`
- `<blockquote>`
- `<canvas>`
- `<dd>`
- `<div>`
- `<dl>`
- `<dt>`
- `<fieldset>`
- `<figcaption>`
- `<figure>`
- `<footer>`
- `<form>`
- `<h1>-<h6>`
- `<header>`
- `<hr>`
- `<li>`
- `<main>`
- `<nav>`
- `<noscript>`
- `<ol>`
- `<p>`
- `<pre>`
- `<section>`
- `<table>`
- `<tfoot>`
- `<ul>`
- `<video>`

------

## Inline Elements

인라인 엘리먼트는 새로운 라인을 시작하지 않고 필요한 넓이만큼을 가져간다.

### 예제

```html
<span>Hello World</span>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_inline_span)

HTML에서 인라인 엘리먼트는 다음과 같다.

------

## The <div> Element

`<div>`엘리먼트는 종종 HTMl의 컨테이너로 사용된다.

`<div>`엘리먼트는 요구되는 속성이 없다. 그러나 style, class, id는 공통적으로 있다.

CSS와 같이 사용할때 `<div>`엘리먼트는 내용의 스타일 블록으로 사용될 수 있다.

### 예제

```html
<div style="background-color:black;color:white;padding:20px;">
  <h2>London</h2>
  <p>London is the capital city of England. It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
</div>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_div_capitals)

------

## The <span> Element

`<span>`엘리먼트는 종종 몇몇 텍스트의 컨테이너로 사용된다.

`<span>`엘리먼트는 요구되는 속성은 없지만 style, class, id는 공통이다.

CSS를 사용할때 `<span>`엘리먼트는 텍스트의 스타일부분으로 사용될 수 있다.

### Example

```html
<h1>My <span style="color:red">Important</span> Heading</h1>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_span_red)

------

## HTML Grouping Tags

| 태그     | 설명                                 |
| :------- | :----------------------------------- |
| `<div>`  | 문서에 섹션을 정의한다.(블록 수준)   |
| `<span>` | 문서에 섹션을 정의한다.(인라인 수준) |

[HTML class](./HTML_classattribute.md)

