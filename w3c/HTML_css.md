# HTML Styles - CSS

## CSS로 HTML 스타일링 하기

CSS는 Cascading Style Sheets의 약자입니다.

CSS는 어떻게 HTML 엘리먼트들이 화면이나, 종이 또는 다른 미디어에 어떻게 보여질지를 결정합니다.

CSS는 많은 양의 일들을 줄여줍니다. 이것은 많은 수의 웹페이지를 한번에 통제할 수 있게 해줍니다.

CSS는 3가지 방법으로 HTML 엘리먼트에 추가될 수 있습니다.

- **Inline** - HTML엘리먼트 안의 style 속성을 사용하는 것
- **Internal** - `<head>`섹션 안의 `<style>`엘리먼트를 사용하는 것
- **External** - 외부 CSS 파일을 사용하는 것

CSS를 추가하는 가장 일반적인 방법은 CSS파일을 분리하여 스타일을 정하는 것입니다. 그러나 우리가 inline과 internal styling을 사용할 때도 있습니다. 왜냐하면 이것은 설명하기 쉽고 너 자신이 이것을 시도하기에 쉽기 때문입니다.

**Tip** : 당신은 CSS Tutorial에서 더 많은 것을 배울 수 있습니다.

------

## Inline CSS

하나의 HTML 엘리먼트에서 독특한 스타일을 적용할 때 쓰입니다.

inline CSS 는 HTML 엘리먼트의 스타일속성을 사용합니다.

아래 예제는 h1 엘리먼트의 텍스트 색상을 파란색으로 바꾸는 것입니다.

### 예제

```html
<h1 style="color:blue;">This is a Blue Heading</h1>
```



## Internal CSS

internal CSS는 단일 HTML 페이지의 CSS를 정의할 때 사용합니다.

internal CSS는 HTML 페이지의 `<head>`섹션에서 정의되고 `<style>`엘리먼트이내에 정의됩니다.

### 예제

```html
<!DOCTYPE html>
<html>
<head>
<style>
body {background-color: powderblue;}
h1  {color: blue;}
p  {color: red;}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

------

## External CSS

외부 스타일 시트는 많은 HTML 페이지의 스타일을 정의할 때 사용됩니다.

또한 외부 스타일시트에서 당신은 단지 하나의 파일을 바꿈으로써 전체 웹사이트의 모습을 변화 시킬 수 있습니다.

아래의 예제는 HTML페이지의 섹션 `<head>`에 링크를 추가하는 예제 입니다.

### 예제

```html
<!DOCTYPE html>
<html>
<head>
 <link rel="stylesheet" href="styles.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```



외부 스타일시트는 어떠한 텍스트 에디터에서도 쓰일 수 있습니다. 이 파일은 어떠한 HTML 코드도 포함해서는 안되며 단지 .css 확장파일명으로 저장되기만 하면 됩니다.

아래는 "style.css"가 어떻게 쓰이는지 보입니다.

```css
body {
 background-color: powderblue;
}
h1 {
 color: blue;
}
p {
 color: red;
}
```



------

## CSS Fonts

CSS `color`속성은 텍스트 칼라를 정의한다.

CSS `font-family`속성은 사용될 폰트를 정의한다.

CSS `font-size`속성은 사용될 폰트의 크기를 정의한다.

### 예제

```html
<!DOCTYPE html>
<html>
<head>
<style>
h1 {
 color: blue;
 font-family: verdana;
 font-size: 300%;
}
p {
 color: red;
 font-family: courier;
 font-size: 160%;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```



------

## CSS Border

CSS border속성은 HTML엘리먼트의 테두리를 정하는 것이다.

### 예제

```css
p {
 border: 1px solid powderblue;
}
```

------

## CSS Padding

CSS 패딩속성은 텍스트와 테두리 사이의 공간의 크기를 지정하는 것이다.

### 예제

```css
p {
 border: 1px solid powderblue;
 padding: 30px;
}
```



------

## CSS Margin

CSS 마진은 테두리의 밖의 공간의 크기를 정의하는 것이다.

### 예제

```css
p {
 border: 1px solid powderblue;
 margin: 50px;
}
```



------

## The id Attribute

하나의 특수한 엘리먼트의 스타일을 정의하기 위해서는 엘리먼트의 속성에 id 를쓴다.

```html
<p id="p01">I am different</p>
```

그때 특수한 아이디의 스타일을 정의하면 된다.

### 예제

```css
#p01 {
 color: blue;
}
```



**Note:** 페이지 이내에 엘리먼트의 아이디는 오직 하나여야만 하고, 그래서 아이디 선택자는 하나의 특수한 엘리먼트만 선택할 수 있어야 한다.

------

## The class Attribute

엘리먼트의 특수한 속성을 정의하기 위해서 엘리먼트의 클래스 속성을 추가해라

```html
<p class="error">I am different</p>
```

그때 특수한 클래스의 엘리먼트에 대한 스타일을 정의하면 된다.

### 예제

```css
p.error {
 color: red;
}
```



------

## 외부 참조

외부 스타일 시트는 URL 경로를 통해 참조 될 수 있다. 또한 현재 웹페이지의 상대 참조로도 가능하다. 아래는 스타일시트의 URL에 대한 링크이다.

### 예제

```css
<link rel="stylesheet" href="https://www.w3schools.com/html/styles.css">
```

아래의 예제는 현재 웹사이트의 html 폴더에 위치한 스타일시트에 대한 링크이다.

### 예제

```css
<link rel="stylesheet" href="/html/styles.css">
```



아래의 예제는 현재 웹페이지와 같은 폴더에 있는 스타일시트에 대한 링크이다.

### 예제

```css
<link rel="stylesheet" href="styles.css">
```



당신은 다음과 같은 링크에서 이에 대한 더 자세한 사항을 볼 수 있다. [HTML File Paths](https://www.w3schools.com/html/html_filepaths.asp).

------

## 챕터 요약

- inline 스타일링을 위해서는 style 속성을 사용해라
- internal 스타일링을 위해서는 `<style>`속성을 사용해라
- external 스타일링을 위해서는 `<link>`속성을 사용해라
- style과 link 엘리먼트를 저장하기 위해서는 `<head>`엘리먼트를 사용해라
- 텍스트 색상을 지정하기 위해서는 `color`속성을 사용해라
- 텍스트 폰트를 지정하기 위해서는 `font-family` 를 사용해라
- 텍스트 폰트의 크기를 지정하기 위해서는  `font-size` 를 사용해라
- 테두리의 속성을 지정하기 위해서는  `border` 를 사용해라
- 테두리 안의 공간의 속성을 지정하기 위해서는 `padding`을 사용해라
- 테두리 밖의 공간의 속성을 지정하기 위해서는`margin` 을 사용해라

## HTML Style Tags

| 태그      | 설명                                     |
| :-------- | :--------------------------------------- |
| `<style>` | HTML 문서를 위한 스타일 정보를 정의한다. |
| `<link>`  | 문서와 외부소스 사이의 링크를 정의한다.  |

[HTML Links](/HTML_links.md)