# CSS Pseudo-classes

## Pseudo-classes란 무엇인가?

A pseudo-class는 엘리먼트의 특수한 상태를 정하는데 사용된다.

예를들어 그것은 다음과 같이 사용될 수 있다.

- 마우스가 엘리먼트에 올라갈 때 엘리먼트의 스타일을 지정함
- 방문한 링크와 방문하지않은 링크를 다르게 스타일 지정함.
- 그것이 포커스 될 때 스타일이 바뀜.

Mouse Over Me



------

## 문법

pseudo-classes의 문법이다.

```css
selector:pseudo-class {
 property:value;
}
```



------

## Anchor Pseudo-classes

링크는 다른 방식으로 보여질 수 있다.

### 예제

```css
/* unvisited link */
a:link {
 color: #FF0000;
}

/* visited link */
a:visited {
 color: #00FF00;
}

/* mouse over link */
a:hover {
 color: #FF00FF;
}

/* selected link */
a:active {
 color: #0000FF;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_link)

**Note:** CSS 정의에서`a : hover`는`a : link`와`a : visited`뒤에 와야 효과적이다! `a : active`는 CSS 정의에서`a : hover` 뒤에 와야 효과적이다! 의사 클래스 이름은 대소 문자를 구분하지 않는다.

------

## Pseudo-classes and CSS Classes

Pseudo- class는 CSS 클래스들과 결합될 수 있다.

예제에서 링크 위로 마우스를 가져가면 색상이 변경된다.

### 예제

```css
a.highlight:hover {
 color: #ff0000;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_pseudo-class)

------

## Hover on `<div>`

`<div>` 요소에서 : hover 의사 클래스를 사용하는 예 :

### 예제

```css
div:hover {
 background-color: blue;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_pseudo-class_hover_div)

------

## Simple Tooltip Hover

`<div>` 요소 위로 마우스를 가져 가면 툴팁과 같은 `<p>` 요소가 표시된다.

### 예제

```css
p {
 display: none;
 background-color: yellow;
 padding: 20px;
}

div:hover p {
 display: block;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_pseudo-class_hover_tooltip)

------

## CSS - The :first-child Pseudo-class

`: first-child` 의사 클래스는 다른 요소의 첫 번째 자식 인 지정된 요소와 일치한다.

## Match the first `<p>` element

다음 예제에서 선택기는 요소의 첫 번째 자식 인 `<p>` 요소와 일치한다.

### 예제

```css
p:first-child {
 color: blue;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_first-child1)

------

## Match the first `<i>` element in all `<p>` elements

다음 예에서 선택기는 `<p>`엘리먼트의 첫 번째 `<i>`엘리먼트를 선택한다.

### 예제

```css
p i:first-child {
 color: blue;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_first-child2)

------

## Match all `<i>` elements in all first child `<p>` elements

다음 예에서 선택기는 다른 요소의 첫 번째 자식 인 `<p>` 엘리먼트의 모든 `<i> `엘리먼트를 선택한다.

### 예제

```css
p:first-child i {
 color: blue;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_first-child3)

------

## CSS - The :lang Pseudo-class

: lang 의사 클래스를 사용하면 다른 언어에 대한 특수 규칙을 정의 할 수 있다.

아래 예에서 : lang은 lang = "no"를 사용하여 <q> 요소의 인용 부호를 정의한다.

### 예제

```css
<html>
<head>
<style>
q:lang(no) {
 quotes: "~" "~";
}
</style>
</head>
<body>

<p>Some text <q lang="no">A quote in a paragraph</q> Some text.</p>

</body>
</html>
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_lang)

------

## All CSS Pseudo Classes

| Selector                                                     | Example               | 예제                                                         |
| :----------------------------------------------------------- | :-------------------- | :----------------------------------------------------------- |
| [:active](https://www.w3schools.com/cssref/sel_active.asp)   | a:active              | 활성 링크를 선택                                             |
| [:checked](https://www.w3schools.com/cssref/sel_checked.asp) | input:checked         | 검사 된 모든 <input> 요소를 선택                             |
| [:disabled](https://www.w3schools.com/cssref/sel_disabled.asp) | input:disabled        | 비활성화 된 모든 <input> 요소를 선택                         |
| [:empty](https://www.w3schools.com/cssref/sel_empty.asp)     | p:empty               | 자식이없는 모든 `<p>` 요소를 선택                            |
| [:enabled](https://www.w3schools.com/cssref/sel_enabled.asp) | input:enabled         | 활성화 된 모든 `<input>` 요소를 선택                         |
| [:first-child](https://www.w3schools.com/cssref/sel_firstchild.asp) | p:first-child         | 부모의 첫 번째 자식 인 모든 `<p>` 요소를 선택                |
| [:first-of-type](https://www.w3schools.com/cssref/sel_first-of-type.asp) | p:first-of-type       | 부모의 첫 번째 `<p>` 요소 인 모든 `<p>` 요소를 선택          |
| [:focus](https://www.w3schools.com/cssref/sel_focus.asp)     | input:focus           | 포커스가있는 `<input>` 요소를 선택                           |
| [:hover](https://www.w3schools.com/cssref/sel_hover.asp)     | a:hover               | 마우스 오버 링크를 선택                                      |
| [:in-range](https://www.w3schools.com/cssref/sel_in-range.asp) | input:in-range        | 지정된 범위 내의 값을 가진 `<input>` 요소를 선택             |
| [:invalid](https://www.w3schools.com/cssref/sel_invalid.asp) | input:invalid         | 유효하지 않은 값을 가진 모든 `<input>` 요소를 선택           |
| [:lang(*language*)](https://www.w3schools.com/cssref/sel_lang.asp) | p:lang(it)            | "it"로 시작하는 lang 속성 값을 가진 모든 `<p> `요소를 선택합니다. |
| [:last-child](https://www.w3schools.com/cssref/sel_last-child.asp) | p:last-child          | 부모의 마지막 자식 인 모든 `<p>` 요소를 선택                 |
| [:last-of-type](https://www.w3schools.com/cssref/sel_last-of-type.asp) | p:last-of-type        | 부모의 마지막 `<p>` 요소 인 모든 `<p>` 요소를 선택           |
| [:link](https://www.w3schools.com/cssref/sel_link.asp)       | a:link                | 방문하지 않은 모든 링크를 선택                               |
| [:not(selector)](https://www.w3schools.com/cssref/sel_not.asp) | :not(p)               | `<p>` 요소가 아닌 모든 요소를 선택                           |
| [:nth-child(n)](https://www.w3schools.com/cssref/sel_nth-child.asp) | p:nth-child(2)        | 부모의 두 번째 자식 인 모든 `<p>` 요소를 선택                |
| [:nth-last-child(n)](https://www.w3schools.com/cssref/sel_nth-last-child.asp) | p:nth-last-child(2)   | 마지막 자식부터 세어 부모의 두 번째 자식 인 모든 `<p>` 요소를 선택 |
| [:nth-last-of-type(n)](https://www.w3schools.com/cssref/sel_nth-last-of-type.asp) | p:nth-last-of-type(2) | 마지막 자식부터 세어 부모의 두 번째 `<p>` 요소 인 모든 `<p>` 요소를 선택 |
| [:nth-of-type(n)](https://www.w3schools.com/cssref/sel_nth-of-type.asp) | p:nth-of-type(2)      | 부모의 두 번째 `<p>` 요소 인 모든 `<p>` 요소를 선택          |
| [:only-of-type](https://www.w3schools.com/cssref/sel_only-of-type.asp) | p:only-of-type        | 부모의 유일한 `<p>` 요소 인 모든 `<p>` 요소를 선택합니다.    |
| [:only-child](https://www.w3schools.com/cssref/sel_only-child.asp) | p:only-child          | 부모의 유일한 자식 인 모든 `<p>` 요소를 선택합니다           |
| [:optional](https://www.w3schools.com/cssref/sel_optional.asp) | input:optional        | "필수"속성이없는 `<input>` 요소를 선택                       |
| [:out-of-range](https://www.w3schools.com/cssref/sel_out-of-range.asp) | input:out-of-range    | 지정된 범위 밖의 값을 가진 `<input>` 요소를 선택             |
| [:read-only](https://www.w3schools.com/cssref/sel_read-only.asp) | input:read-only       | "읽기 전용"속성이 지정된`<input>`요소를 선택                 |
| [:read-write](https://www.w3schools.com/cssref/sel_read-write.asp) | input:read-write      | "읽기 전용"속성이없는`<input>`요소를 선택                    |
| [:required](https://www.w3schools.com/cssref/sel_required.asp) | input:required        | "필수"속성이 지정된`<input>`요소를 선택                      |
| [:root](https://www.w3schools.com/cssref/sel_root.asp)       | root                  | 문서의 루트 요소를 선택                                      |
| [:target](https://www.w3schools.com/cssref/sel_target.asp)   | #news:target          | 현재 활성 #news 요소를 선택 (해당 앵커 이름이 포함 된 URL을 클릭 함) |
| [:valid](https://www.w3schools.com/cssref/sel_valid.asp)     | input:valid           | 유효한 값을 가진 모든 `<input>` 요소를 선택합니다            |
| [:visited](https://www.w3schools.com/cssref/sel_visited.asp) | a:visited             | 방문한 모든 링크를 선택                                      |

## All CSS Pseudo Elements

| Selector                                                     | Example         | Example description                 |
| :----------------------------------------------------------- | :-------------- | :---------------------------------- |
| [::after](https://www.w3schools.com/cssref/sel_after.asp)    | p::after        | 모든 `<p>` 요소 뒤에 내용 삽입      |
| [::before](https://www.w3schools.com/cssref/sel_before.asp)  | p::before       | 모든 `<p>` 요소 앞에 내용 삽입      |
| [::first-letter](https://www.w3schools.com/cssref/sel_firstletter.asp) | p::first-letter | 모든 `<p>` 요소의 첫 글자를 선택    |
| [::first-line](https://www.w3schools.com/cssref/sel_firstline.asp) | p::first-line   | 모든 `<p>` 요소의 첫 번째 줄을 선택 |
| [::selection](https://www.w3schools.com/cssref/sel_selection.asp) | p::selection    | 사용자가 선택한 요소 부분을 선택    |

[CSS Pseudo-elements](./CSS_pseudoelements.md)