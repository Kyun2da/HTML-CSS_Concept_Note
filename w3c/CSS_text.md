# CSS Text

## 텍스트 색상

`color`속성은 텍스트의 색상을 지정하는데 사용된다. 색상은 다음에 의해 특화된다.

-  "red"같은 색깔 이름
- "#ff0000"같은 hex값
- "rgb(255,0,0)"값 같은 rgb값

 [CSS Color Values](https://www.w3schools.com/cssref/css_colors_legal.asp) 가능한 칼라값의 리스트를 보고싶으면 왼쪽의 링크를 따라가라

페이지의 색상 기본값은 body 선택자 안에 정의되어 있다.

### 예제

```css
body {
 color: blue;
}

h1 {
 color: green;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_color)

**Note:** 만약 너가 `color`속성을 정의한다면 너는 `background-color`를 정의해야만 한다.

------

## Text Alignment

 `text-align` 속성은 텍스트의 수평정렬을 정의하는데에 사용된다.

텍스트는 왼쪽, 오른쪽, 중앙, justified 정렬이 될 수 있다.

다음의 예제는 중앙 정렬, 왼쪽, 오른쪽 정렬을 보여준다.

### 예제

```css
h1 {
 text-align: center;
}

h2 {
 text-align: left;
}

h3 {
 text-align: right;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_text-align)

`text-align`속성이 justify로 두어질 때  모든 줄의 넓이가 같고 잡지 및 신문과 같이 왼쪽과 오른쪽 여백이 똑 바르도록 각 줄이 늘어난다.

### 예제

```css
div {
 text-align: justify;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_text-align_all)



------

## Text Decoration

 `text-decoration` 속성은 텍스트로부터 데코레이션을 제거하거나 셋팅하는데 사용된다.

 `text-decoration: none;` 값은 종종 링크로부터 밑줄을 제거하는데 사용된다.

### 예제

```css
a {
 text-decoration: none;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_text-decoration_link)

 `text-decoration` 값들은 텍스트를 꾸미는데 사용된다.

### 예제

```css
h1 {
 text-decoration: overline;
}

h2 {
 text-decoration: line-through;
}

h3 {
 text-decoration: underline;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_text-decoration)

**Note:** 이것은 링크가 아닌 텍스트의 밑줄을 위해서는 추천되지 않는다. 그것은 오히려 독자에게 혼란을 일으킨다.

------

## Text Transformation

 `text-transform` 속성은 텍스트에 소문자와 대문자에 특화된다.

이것은 대문자 혹은 소문자로 바꾸거나 각 단어의 첫 글자를 대문자로 쓰는데 사용할 수 있다.

### 예제

```css
p.uppercase {
 text-transform: uppercase;
}

p.lowercase {
 text-transform: lowercase;
}

p.capitalize {
 text-transform: capitalize;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_text-transform)

------

## Text Indentation

 `text-indent` 속성은 텍스트의 첫번째 라인의 들여쓰기를 하는데에 특화되어 있다.

### 예제

```css
p {
 text-indent: 50px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_text-indent)

------

## Letter Spacing

 `letter-spacing` 속성은 텍스트에 문자사이에 공간을 정의하는데 특화되어 있다.

다음의 에제는 어떻게 두개의 문자사이의 공간을 늘리거나 줄이는지 보여준다.

### 예제

```css
h1 {
 letter-spacing: 3px;
}

h2 {
 letter-spacing: -3px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_letter-spacing)

------

## Line Height

 `line-height` 속성은 두개의 라인사이의 공간을 정의하는데 특화되어 있다.

### 예제

```css
p.small {
 line-height: 0.8;
}

p.big {
 line-height: 1.8;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_line-height)

------

## Text Direction

 `direction` 속성은 엘리먼트의 텍스트 방향을 변화시키는데 사용된다.

### 예제

```css
p {
 direction: rtl;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_text_direction)

------

## Word Spacing

 `word-spacing` 속성은 텍스트에 단어 사이에 공간을 특화하는데 사용된다.

다음의 에제는 두개의 단어사이의 공간을 어떻게 늘리거나 줄이는지를 보여준다.

### 예제

```css
h1 {
 word-spacing: 10px;
}

h2 {
 word-spacing: -5px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_text_word-spacing)

------

## Text Shadow

 `text-shadow` 속성은 텍스트에 그림자를 추가한다.

다음의 예제는 수평 그림자의 위치와 수직 그림자의 위치, 그림자의 색깔을 변화시키는 것을 보여준다.

### 예제

```css
h1 {
 text-shadow: 3px 2px red;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_text-shadow)

------

## All CSS Text Properties

| Property                                                     | Description                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [color](https://www.w3schools.com/cssref/pr_text_color.asp)  | 텍스트의 색깔을 세팅한다.                                    |
| [direction](https://www.w3schools.com/cssref/pr_text_direction.asp) | 방향이나 쓰기 방향을 설정한다.                               |
| [letter-spacing](https://www.w3schools.com/cssref/pr_text_letter-spacing.asp) | 텍스트에 사이의 문자의 공간을 늘리거나 줄인다.               |
| [line-height](https://www.w3schools.com/cssref/pr_dim_line-height.asp) | 라인 높이를 설정한다.                                        |
| [text-align](https://www.w3schools.com/cssref/pr_text_text-align.asp) | 텍스트의 수평정렬을 설정한다.                                |
| [text-decoration](https://www.w3schools.com/cssref/pr_text_text-decoration.asp) | 텍스트에 꾸미는 것을 설정한다.                               |
| [text-indent](https://www.w3schools.com/cssref/pr_text_text-indent.asp) | 텍스트 블록에 첫번째 라인의 들여쓰기를 설정한다.             |
| [text-shadow](https://www.w3schools.com/cssref/css3_pr_text-shadow.asp) | 텍스트에 그림자 효과를 추가한다.                             |
| [text-transform](https://www.w3schools.com/cssref/pr_text_text-transform.asp) | 텍스트의 대문자를 통제한다.                                  |
| [text-overflow](https://www.w3schools.com/cssref/css3_pr_text-overflow.asp) | 유저에게 표시되지않는 오버플로우 컨텐츠를 알리는 방법을 지정한다. |
| [unicode-bidi](https://www.w3schools.com/cssref/pr_text_unicode-bidi.asp) | direction 속성과 함께 사용하여 동일한 문서에서 여러 언어를 지원하도록 텍스트를 재정의할지 여부를 설정하거나 반환한다. |
| [vertical-align](https://www.w3schools.com/cssref/pr_pos_vertical-align.asp) | 엘리먼트의 수직 정렬을 설정한다.                             |
| [white-space](https://www.w3schools.com/cssref/pr_text_white-space.asp) | 어떻게 엘리먼트안의 하얀색 공간을 다룰지를 결정한다.         |
| [word-spacing](https://www.w3schools.com/cssref/pr_text_word-spacing.asp) | 단어 사이의 공간을 늘리거나 줄인다                           |

[CSS Fonts](./CSS_Fonts.md)

