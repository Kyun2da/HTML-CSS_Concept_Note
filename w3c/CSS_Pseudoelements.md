# CSS Pseudo-elements

## What are Pseudo-Elements?

CSS pseudo-element는 엘리먼트의 특수한 부분의 스타일을 지정하는 것이다.

예를들어 이것은 다음과 같이 사용된다.

- 엘리먼트의 첫글자, 라인, 글자등을 스타일링한다.
- 엘리먼트의 내용 전 혹은 후에 내용을 삽입한다.

------

## 문법

pseudo-element의  문법

```css
selector::pseudo-element {
 property:value;
}
```

**이중 콜론 표기법에주의!** `:: first-line` vs`: first-line`

이중 콜론은 CSS3에서 의사 요소의 단일 콜론 표기법을 대체했다. 이것은 **의사 클래스 **와 **의사 요소 **를 구별하기위한 W3C의 시도였다.

단일 콜론 구문은 CSS2 및 CSS1의 유사 클래스 및 유사 요소 모두에 사용되었다.

이전 버전과의 호환성을 위해 단일 콜론 구문은 CSS2 및 CSS1 의사 요소에 허용된다.

------

## The ::first-line Pseudo-element

`:: first-line` 의사 요소는 텍스트의 첫 줄에 특수 스타일을 추가하는 데 사용된다.

다음 예제는 모든 `<p>` 요소에서 텍스트의 첫 줄을 형식화한다.

### 예제

```css
p::first-line {
 color: #ff0000;
 font-variant: small-caps;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_firstline)

**Note:** `:: first-line` 유사 요소는 블록 수준 요소에만 적용 할 수 있다.

다음 속성은`:: first-line` 유사 요소에 적용된다.

- font properties
- color properties
- background properties
- word-spacing
- letter-spacing
- text-decoration
- vertical-align
- text-transform
- line-height
- clear

------

## The ::first-letter Pseudo-element

`:: first-letter` 유사 요소는 텍스트의 첫 글자에 특수 스타일을 추가하는 데 사용된다.

다음 예제는 모든 `<p>` 요소에서 텍스트의 첫 문자를 형식화한다.

### 예제

```css
p::first-letter {
 color: #ff0000;
 font-size: xx-large;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_firstletter)

**Note:**  `:: first-letter` 유사 요소는 블록 레벨 요소에만 적용 할 수 있다.

다음 속성은 :: first-letter pseudo- element에 적용된다.

- font properties
- color properties 
- background properties
- margin properties
- padding properties
- border properties
- text-decoration
- vertical-align (only if "float" is "none")
- text-transform
- line-height
- float
- clear

------

## Pseudo-elements and CSS Classes

 의사 요소는 CSS 클래스와 결합 될 수 있다.

### 예제

```css
p.intro::first-letter {
 color: #ff0000;
 font-size:200%;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_pseudo-element)

위의 예는 class = "intro"가있는 단락의 첫 글자를 빨간색과 큰 크기로 표시한다.

------

## Multiple Pseudo-elements

여러 의사 요소도 결합 할 수 있다.

다음 예에서 단락의 첫 문자는 xx- 큰 글꼴 크기에서 빨간색이다. 첫 번째 줄의 나머지 부분은 파란색이며 작은 대문자로 표시된다. 나머지 단락은 기본 글꼴 크기 및 색상이된다.

### 예제

```css
p::first-letter {
 color: #ff0000;
 font-size: xx-large;
}

p::first-line {
 color: #0000ff;
 font-variant: small-caps;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_firstline_letter)

------

## CSS - The ::before Pseudo-element

`:: before` pseudo-element는 요소의 내용 앞에 일부 내용을 삽입하는 데 사용될 수 있다.

다음 예제는 각`<h1>`요소의 내용 앞에 이미지를 삽입한다.

### 예제

```css
h1::before {
 content: url(smiley.gif);
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_before)

------

## CSS - The ::after Pseudo-element

`:: after` 유사 요소는 요소의 내용 뒤에 일부 내용을 삽입하는 데 사용할 수 있다.

다음 예제는 각 `<h1>` 요소의 내용 뒤에 이미지를 삽입한다.

### 예제

```css
h1::after {
 content: url(smiley.gif);
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_after)

------

## CSS - The ::selection Pseudo-element

`:: selection` 의사 요소는 사용자가 선택한 요소 부분과 일치한다.

`:: selection` :`color`,`background`,`cursor` 및`outline`에 다음 CSS 속성을 적용 할 수 있습니다.

다음 예제는 선택한 텍스트를 노란색 배경에서 빨간색으로 만든다.

### 예제

```css
::selection {
 color: red;
 background: yellow;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss3_selection)

## All CSS Pseudo Elements

| Selector                                                     | 예제            | 설명                                |
| :----------------------------------------------------------- | :-------------- | :---------------------------------- |
| [::after](https://www.w3schools.com/cssref/sel_after.asp)    | p::after        | 각 <p> 요소의 내용 뒤에 무언가 삽입 |
| [::before](https://www.w3schools.com/cssref/sel_before.asp)  | p::before       | 각 <p> 요소의 내용 앞에 무언가 삽입 |
| [::first-letter](https://www.w3schools.com/cssref/sel_firstletter.asp) | p::first-letter | 각 <p> 요소의 첫 글자를 선택        |
| [::first-line](https://www.w3schools.com/cssref/sel_firstline.asp) | p::first-line   | 각 <p> 요소의 첫 번째 줄을 선택     |
| [::selection](https://www.w3schools.com/cssref/sel_selection.asp) | p::selection    | 사용자가 선택한 요소 부분을 선택    |

## All CSS Pseudo Classes

| Selector                                                     | 예제                  | 설명                                                         |
| :----------------------------------------------------------- | :-------------------- | :----------------------------------------------------------- |
| [:active](https://www.w3schools.com/cssref/sel_active.asp)   | a:active              | 활성 링크를 선택                                             |
| [:checked](https://www.w3schools.com/cssref/sel_checked.asp) | input:checked         | 검사 된 모든 `<input>` 요소를 선택                           |
| [:disabled](https://www.w3schools.com/cssref/sel_disabled.asp) | input:disabled        | 비활성화 된 모든 `<input>` 요소를 선택                       |
| [:empty](https://www.w3schools.com/cssref/sel_empty.asp)     | p:empty               | 자식이없는 모든 `<p>` 요소를 선택                            |
| [:enabled](https://www.w3schools.com/cssref/sel_enabled.asp) | input:enabled         | 활성화 된 모든 `<input>` 요소를 선택                         |
| [:first-child](https://www.w3schools.com/cssref/sel_firstchild.asp) | p:first-child         | 부모의 첫 번째 자식 인 모든 `<p>` 요소를 선택                |
| [:first-of-type](https://www.w3schools.com/cssref/sel_first-of-type.asp) | p:first-of-type       | 부모의 첫 번째 `<p>` 요소 인 모든 `<p>` 요소를 선택          |
| [:focus](https://www.w3schools.com/cssref/sel_focus.asp)     | input:focus           | 포커스가있는 `<input>` 요소를 선택                           |
| [:hover](https://www.w3schools.com/cssref/sel_hover.asp)     | a:hover               | 마우스 오버 링크를 선택                                      |
| [:in-range](https://www.w3schools.com/cssref/sel_in-range.asp) | input:in-range        | 지정된 범위 내의 값을 가진 `<input>` 요소를 선택             |
| [:invalid](https://www.w3schools.com/cssref/sel_invalid.asp) | input:invalid         | 유효하지 않은 값을 가진 모든 `<input>` 요소를 선택           |
| [:lang(*language*)](https://www.w3schools.com/cssref/sel_lang.asp) | p:lang(it)            | "it"로 시작하는 lang 속성 값을 가진 모든 `<p>` 요소를 선택   |
| [:last-child](https://www.w3schools.com/cssref/sel_last-child.asp) | p:last-child          | 부모의 마지막 자식 인 모든 `<p>` 요소를 선택                 |
| [:last-of-type](https://www.w3schools.com/cssref/sel_last-of-type.asp) | p:last-of-type        | 부모의 마지막 `<p>` 요소 인 모든 `<p>` 요소를 선택           |
| [:link](https://www.w3schools.com/cssref/sel_link.asp)       | a:link                | 방문하지 않은 모든 링크를 선택                               |
| [:not(selector)](https://www.w3schools.com/cssref/sel_not.asp) | :not(p)               | `<p>` 요소가 아닌 모든 요소를 선택                           |
| [:nth-child(n)](https://www.w3schools.com/cssref/sel_nth-child.asp) | p:nth-child(2)        | 부모의 두 번째 자식 인 모든 `<p>` 요소를 선택                |
| [:nth-last-child(n)](https://www.w3schools.com/cssref/sel_nth-last-child.asp) | p:nth-last-child(2)   | 마지막 자식부터 세어 부모의 두 번째 자식 인 모든 `<p>` 요소를 선택 |
| [:nth-last-of-type(n)](https://www.w3schools.com/cssref/sel_nth-last-of-type.asp) | p:nth-last-of-type(2) | 마지막 자식부터 세어 부모의 두 번째 `<p>` 요소 인 모든 `<p>` 요소를 선택 |
| [:nth-of-type(n)](https://www.w3schools.com/cssref/sel_nth-of-type.asp) | p:nth-of-type(2)      | 부모의 두 번째 `<p>` 요소 인 모든 `<p>` 요소를 선택          |
| [:only-of-type](https://www.w3schools.com/cssref/sel_only-of-type.asp) | p:only-of-type        | 부모의 유일한 `<p>` 요소 인 모든 `<p>` 요소를 선택           |
| [:only-child](https://www.w3schools.com/cssref/sel_only-child.asp) | p:only-child          | 부모의 유일한 자식 인 모든 `<p>` 요소를 선택                 |
| [:optional](https://www.w3schools.com/cssref/sel_optional.asp) | input:optional        | "필수"속성이없는 `<input>` 요소를 선택                       |
| [:out-of-range](https://www.w3schools.com/cssref/sel_out-of-range.asp) | input:out-of-range    | 지정된 범위 밖의 값을 가진 `<input>` 요소를 선택             |
| [:read-only](https://www.w3schools.com/cssref/sel_read-only.asp) | input:read-only       | "읽기 전용"속성이 지정된 `<input>` 요소를 선택               |
| [:read-write](https://www.w3schools.com/cssref/sel_read-write.asp) | input:read-write      | "읽기 전용"속성이없는 `<input>` 요소를 선택                  |
| [:required](https://www.w3schools.com/cssref/sel_required.asp) | input:required        | "필수"속성이 지정된 `<input>` 요소를 선택                    |
| [:root](https://www.w3schools.com/cssref/sel_root.asp)       | root                  | 문서의 루트 요소를 선택                                      |
| [:target](https://www.w3schools.com/cssref/sel_target.asp)   | #news:target          | 현재 활성 #news 요소를 선택 (해당 앵커 이름이 포함 된 URL을 클릭 함) |
| [:valid](https://www.w3schools.com/cssref/sel_valid.asp)     | input:valid           | 유효한 값을 가진 모든 <input> 요소를 선택                    |
| [:visited](https://www.w3schools.com/cssref/sel_visited.asp) | a:visited             | 방문한 모든 링크를 선택                                      |

[CSS Opacity](./CSS_opacity.md)