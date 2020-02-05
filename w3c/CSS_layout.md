# CSS Layout - The display Property

`display`속성은 레이아웃을 통제하는데에 가장 중요한 CSS속성이다.

------

## The display Property

`display`속성은 어떻게 엘리먼트가 보여질지를 결정한다.

모든 HTML엘리먼트는 그것이 어떤 타입의 엘리먼트냐에 따라서 기본 디스플레이 값을 가지고 있다. 기본 display 값은 block 혹은 inline 속성이다.

------

## Block-level Elements

블록 수준의 엘리먼트는 항상 새로운 라인으로 시작하고 full 넓이 값을 가지고 있다.

다음은 블록 엘리먼트의 예이다.

- `<div>`
- `<h1>` - `<h6>`
- `<p>`
- `<form>`
- `<header>`
- `<footer>`
- `<section>`

------

## Inline Elements

인라인 엘리먼트는 새로운 라인으로 시작하지 않고 필요한 넓이만큼만 가진다.

인라인 엘리먼트의 예는 다음과 같다.

- `<span>`
- `<a>`
- `<img>`

------

## Display: none;

`display: none;` 은 일반적으로 자바스크립트에서 엘리먼트를 삭제하거나 다시만들지 않고 보여주지 않을 때 사용한다. 이 페이지의 마지막 예에서 너가 이것이 어떻게 보여질지를 원하면 마지막 예를 보면 된다.

`<script>`엘리먼트는 `display:none`값을 기본적으로 사용한다.

------

## Override The Default Display Value

언급한것 처럼 모든 엘리먼트는 display 기본값을 가지고있다. 그러나 너는 이것을 오버라이드 할 수 있다.

인라인 엘리먼트를 블록 엘리먼트로 바꾸는것 혹은 그반대는 페이지를 특수한 방법으로 보이도록 만들 수 있고 이것은 웹표준에서 허용되고 있다.

### 예제

```css
li {
 display: inline;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_display_inline_list)

**Note:** 엘리먼트의 디스플레이 속성을 세팅하는것은 오직 엘리먼트가 어떻게 보여질지를 바꾸는 것이며 엘리먼트의 종류를 바꾸는 것이 아니다. 그래서 인라인엘리먼트가 `display:block`값을 갖고있더라도 이것은 엘리먼트를 블록으로 바꾸지 않는다.

다음의 예제는 `<span>`엘리먼트를 블록 엘리먼트 처럼 바꾸는 것이다.

### 예제

```css
span {
 display: block;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_display_block)

다음의 예제는 `<a>`엘리먼트를 블록엘리먼트 처럼 바꾸는 것이다.

### 예제

```css
a {
 display: block;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_display_block_a)

엘리먼트를 숨기는 것은 display 속성을 none 으로 바꿈으로써 될 수 있다. 이 엘리먼트는 숨겨질 것이며 페이지는 엘리먼트가 거기에 없는 것 처럼 보일 것이다.

### 예제

```css
h1.hidden {
 display: none;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_display_none)

`visibility:hidden;` 속성은 또한 엘리먼트를 숨긴다.

그러나 이 엘리먼트는 전처럼 같은 공간을 가지고 있다는 것이다. 이 엘리먼트가 숨겨지면 여전히 레이아웃은 그대로일 것이다.

### 예제

```css
h1.hidden {
 visibility: hidden;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_visibility_hidden)

------

## CSS Display/Visibility Properties

| 속성                                                         | 설명                                                         |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [display](https://www.w3schools.com/cssref/pr_class_display.asp) | 어떻게 엘리먼트가 보여질지를 결정한다.                       |
| [visibility](https://www.w3schools.com/cssref/pr_class_visibility.asp) | 엘리먼트가 보일지 말지를 결정한다. 안보여도 레이아웃은 차지한다. |

[CSS Max-width](./CSS_maxwidth.md)