# CSS Links

## Styling Links

링크는 CSS속성에의해 스타일링 될 수 있다. (`color`, `font-family`, `background `등등)

### 예제

```css
a {
 color: hotpink;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_link_all)

또한 링크의 상태에 따라 링크 스타일을 다르게 지정할 수 있다.

네 가지 링크 상태는 다음과 같다.

- `a:link` - 일반적인 방문하지 않은 링크
- `a:visited` - 유저가 방문했던 링크
- `a:hover` - 마우스를 가져다댈때 링크
- `a:active` - 마우스를 클릭할 때 링크

```css
/* unvisited link */
a:link {
 color: red;
}

/* visited link */
a:visited {
 color: green;
}

/* mouse over link */
a:hover {
 color: hotpink;
}

/* selected link */
a:active {
 color: blue;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_link)

몇가지 링크의 상태 스타일을 셋팅할 때 여기에 몇가지 규칙들이 있다.

- a : hover는 반드시 a : link와 a : visited 뒤에 와야한다.
- a:active는 반드시 a:hover 뒤에 와야 한다.

------

## Text Decoration

 `text-decoration` 속성은 대게 링크로부터의 밑줄을 지우는데 사용된다.

### 예제

```css
a:link {
 text-decoration: none;
}

a:visited {
 text-decoration: none;
}

a:hover {
 text-decoration: underline;
}

a:active {
 text-decoration: underline;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_link_decoration)

------

## Background Color

 `background-color` 속성은 대게 링크에 대한 배경색을 변경하는데에 사용된다.

### 예제

```css
a:link {
 background-color: yellow;
}

a:visited {
 background-color: cyan;
}

a:hover {
 background-color: lightgreen;
}

a:active {
 background-color: hotpink;
} 
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_link_background)

------

## Advanced - Link Buttons

이 예제는 좀 더 진보한 예제이다. 우리가 몇몇 CSS 속성들을 이용해 버튼이나 박스를 링크로 사용할 수 있다.

### 예제

```css
a:link, a:visited {
 background-color: #f44336;
 color: white;
 padding: 14px 25px;
 text-align: center;
 text-decoration: none;
 display: inline-block;
}

a:hover, a:active {
 background-color: red;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_link_advanced)



[CSS Lists](./CSS_lists.md)

