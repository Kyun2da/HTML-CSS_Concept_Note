# HTML Links

링크는 거의 모든 웹페이지에서 찾아볼 수 있다. 링크는 유저들이 페이지로부터 다른페이지로 이동하는 방법 중 하나이다.

------

## HTML Links - Hyperlinks

HTML 링크는 하이퍼링크이다.

너가 링크를 클릭하면 다른 문서로 넘어갈 수 있다.

너가 마우스를 링크에 가져다 대면 마우스는 작은 손으로 링크를 가리킬 것이다.

**Note:** 링크는 텍스트만 있는 것이 아니라 그것은 HTML 엘리먼트의 어떤 것이든 될 수 있다. 예를들어 이미지등

------

## HTML Links - Syntax

하이퍼링크는 `<a>`태그로 정의된다.

### 예제

```html
<a href="https://www.w3schools.com/html/">Visit our HTML tutorial</a>
```

 `href` 속성은 링크의 목적지 주소를 적는 속성이다.

링크의 텍스트는 보이는 부분이다.

링크 텍스트를 클릭하면 너를 약속된 주소로 보낼 것이다.

**Note:** 주소의 끝에 슬래시 없이도 너는 아마 서버에 두개의 요청을 할 것이다. 많은 서버들은 자동적으로 주소의 끝에 슬래시를 추가한다. 그리고 그 때 새로운 요청을 보낸다.

------

## Local Links

절대 URL은 아래의 예처럼 사용된다.

지역적 링크는 상대적 URL에서 사용된다.(같은 웹사이트에 링크를 걸 때 사용)

### 예제

```html
<a href="html_images.asp">HTML Images</a>
```



## HTML Links - The target Attribute

 `target `  속성은 문서를 어디에서 열지를 정한다.

 `target` 속성은 다음과 같은 값중 하나가 될 수 있다.

- `_blank` - 새로운 윈도우나 탭에서 링크된 문서를 연다
- `_self` - 그것이 클릭된 같은 윈도우에서 링크된 문서를 연다(기본 값)
- `_parent` - 부모 프레임에서 링크된 문서를 연다
- `_top` - 윈도우의 full body에서 링크된 문서를 연다
- *framename* - 명명된 프레임에서 링크된 문서를 연다

아래 예제는 새로운 윈도우/탭에서 링크된 문서를 여는 예제이다.

### 예제

```html
<a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a>
```



**Tip:** 만약 너의 웹페이지가 프레임에 잠겨있다면 너는 target="_top"을 사용해서 frame이 밖으로 나갈 수 있다.

### 예제

```html
<a href="https://www.w3schools.com/html/" target="_top">HTML5 tutorial!</a>
```



------

## HTML Links - 이미지에 링크를 건다

이것은 이미지에 링크를 거는 예제이다.

### 예제

```html
<a href="default.asp">  <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;border:0;"></a>
```



**Note:** `border:0;` 은 IE9가 이미지 주변에 테두리를 그리는것을 막기위해 사용되었다.(이미지에 링크를 걸 때)

------

## Link Titles

 `title` 속성은 엘리먼트에 관해 추가 정보를 말한다. 이 정보는 엘리먼트에 마우스를 가져다 댈 때 가장 일반적인 툴팁 텍스트로서 보여진다

### 예제

```html
<a href="https://www.w3schools.com/html/" title="Go to W3Schools HTML section">Visit our HTML Tutorial</a>
```



------

## External Paths

외부 페이지는 현재 웹페이지에 fullURL이나 상대경로로 참조될 수 있다.

이 예는 full URL로 웹페이지에 링크를 거는 예제이다.

### 예제

```html
<a href="https://www.w3schools.com/html/default.asp">HTML tutorial</a>
```

아래 예제는 현재 웹사이트에 html 폴더안에있는 위치에 링크를 거는 예제이다.

### 예제

```html
<a href="/html/default.asp">HTML tutorial</a>
```

이 에제는 현재 페이지에 같은 폴더 안에 있는 위치에 링크를 거는 예제이다.

### 예제

```html
<a href="default.asp">HTML tutorial</a>
```

------

## 챕터 요약

- 링크를 걸기위해 `<a>`엘리먼트를 사용하라
- 링크걸 주소를 `href` 태그에 써라
- 링크된 문서를 여는곳을 결정하는데에는  `target` 태그를 사용하라
- 이미지에 링크를 걸때는 `<img>`를 사용해라

## HTML 링크 태그

| 태그  | 설명                   |
| :---- | :--------------------- |
| `<a>` | 하이퍼링크를 정의한다. |

[HTML Images](/HTML_images.md)

