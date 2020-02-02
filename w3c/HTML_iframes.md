# HTML Iframes

------

iframe은 웹페이지 안에 또다른 웹페이지를 보여줄 때 사용한다.

------

## Iframe Syntax

HTML iframe은 `<iframe>`태그로 정의된다.

```html
<iframe src="URL"></iframe>
```

`src`속성은 인라인 프레임 페이지의 URL로 특수화 된다.

------

## Iframe - Set Height and Width

`height`와 `width`속성은 프레임의 사이즈를 정한다.

높이와 넓이는 기본값으로 pixel로 정해진다.

### 예제

```html
<iframe src="demo_iframe.htm" height="200" width="300"></iframe>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_iframe_height_width)

또는 너는 iframe의 넓이와 높이를 정하기 위해서 CSS를 사용할 수 있다.

### 예제

```html
<iframe src="demo_iframe.htm" style="height:200px;width:300px;"></iframe>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_iframe_height_width_css)

------

## Iframe - 테두리 제거

기본적으로 iframe은 그것의 주변에 테두리를 가지고 있다.

테두리를 제거하기 위해서 `style`속성을  추가한고 CSS `border`속성을 사용한다.

### 예제

```html
<iframe src="demo_iframe.htm" style="border:none;"></iframe>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_iframe_frameborder)

CSS에서 너는 크기를 변화시킬 수 있고, iframe의 테두리의 색상과 스타일을 변화시킬 수 있다.

### 예제

```html
<iframe src="demo_iframe.htm" style="border:2px solid red;"></iframe>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_iframe_border2)

## Iframe - 링크 타겟팅 걸기

`iframe`은 링크의 타겟프레임으로 사용될 수 있다.

링크의 `target`속성은 iframe의 `name`속성으로 링크를 걸 수 있다.

### 예제

```html
<iframe src="demo_iframe.htm" name="iframe_a"></iframe>
<p>		
  <a href="https://www.w3schools.com" target="iframe_a">W3Schools.com</a</p>
```

[Try it Yourself »](https://www.w3schools.com/html/exercise.asp?filename=exercise_html_iframe1)

------

## HTML iframe Tag

| 태그       | 설명                      |
| :--------- | :------------------------ |
| `<iframe>` | 인라인 프레임을 정의한다. |

[HTML javascript](./HTML_javascript.md)