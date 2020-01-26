# HTML Attributes (속성)

## HTML 속성들

- 모든 HTML 엘리먼트들은 속성을 갖고있다.
- 속성들은 엘리먼트에 관해 추가적인 정보를 공급한다.
- 속성들은 항상 시작태그에 있다.
- 속성들은 보통 이름과 값이 쌍으로 온다 : name="value"



## href 속성

HTML 링크는 a태그로 정의되어 있다. 이 링크 주소는 href 속성에 적는다.

### 예제

```html
<a href="https://www.w3schools.com">This is a link</a>
```

당신은 튜토리얼에서 a태그와 더많은 링크들을 배울 것이다.



## src 속성

HTML 이미지는 `<img>`태그로 정의되어 있다.

이미지 소스의 파일이름은 `src` 속성에 쓰면 된다

```html
<img src="img_girl.jpg">
```



### 넓이와 높이 속성

HTML 이미지들은 width와  height 속성이 있는데 그것은 이미지의 넓이와 높이를 의미한다.

### 예제

```html
<img src="img_girl.jpg" width="500" height="600">
```



### alt 속성

alt 속성은 만약 이미지가 보일수 없다면 대체해서 나타나는 텍스트를 지정해주는 속성이다.

이 alt속성의 값은 스크린 리더에 의해 읽힐 수 있다. 이 방법은 누군가 웹페이지를 읽을때, 예를들어 시각장애의 사람등이 엘리먼트를 들을 때 사용한다.

```html
<img src="img_girl.jpg" alt="Girl with a jacket">
```

### 예제

만약 이미지가 존재하지 않는다면 무슨일어나는지 한번 봐라

```html
<img src="img_typo.jpg" alt="Girl with a jacket">
```



## 스타일 속성

스타일 속성은 엘리먼트의 스타일을 지정하는데 사용된다. 예를들어 색깔이나 폰트, 사이즈 등등에 사용된다. 요즘은 css때문에 잘 쓰지 않는다.

### 예제

```html
<p style="color:red">This is a paragraph.</p>
```



### lang 속성

`<html>`태그안에 문서의 언어가 선언될 수 있다.

언어는 lang 속성에 선언된다.

언어를 선언하는것은 검색엔진과 어플리케이션의 접근성에 매우 중요하다.

```html
<!DOCTYPE html>
<html lang="en-US">
<body>

...

</body>
</html>
```



### title 속성

`title`  속성은 `<p>`엘리먼트에 추가될 수 있다. title의 속성 값은 너가 단락에 마우스를 가져다 대면 툴팁으로써 보여질 수 있다. 

### 예제

```html
<p title="I'm a tooltip">This is a paragraph.</p>
```



## 소문자 속성을 사용하기를 제안합니다.

HTML5 표준은 소문자 이름을 요구하지않는다.

타이틀 속성은 대문자나 소문자로 쓰일수있다. title of TITLE

w3c는 HTML에서 소문자를 추천하고 XHTML과 같은 문서 타입은 고정적인 소문자를 무조건 요구한다.



## 인용 속성 값을 사용하기를 제안합니다.

 HTML5는 속성값 주변에 인용구를 요구하지 않습니다.

href 속성은 큰따옴표 없이 쓸 수 있습니다.

```html
<a href=https://www.w3schools.com>
```

w3c에서 HTML은 인용구를 추천하지만 XHTML은 고정적으로 인용구를 써야만 합니다.



## 작은따옴표? 큰따옴표?

큰따옴표는 HTML에 가장 일반적으로 쓰이는 값입니다. 그러나 작은따옴표또한 쓰일 수 있습니다.

몇몇 상황에서 우리가 큰따옴표를 포함해야할때, 작은 따옴표의 사용은 필수적입니다.

```html
<p title='John "ShotGun" Nelson'>
```

또는

```html
<p title="John 'ShotGun' Nelson">
```



## 챕터 요약

- 모든 엘리먼트는 속성을 갖습니다.
-  `title` 속성은 추가적인 툴팁 정보를 공급합니다.
-  `href` 속성은 링크를 위해 주소정보를 공급합니다.
-  `width` 와`height` 속성은 이미지의 사이즈 정보에 대한 속성입니다.
- `alt` 속성은 스크린 리더를 위한 텍스트를 공급합니다.
- w3school에서 우리는 항상 소문자 속성이름을 사용합니다.
- w3school에서 우리는 항상 큰따옴표 속성값을 사용합니다.



## HTML 속성

다음은 HTML에서 자주 사용되는 일부 속성을 알파벳순으로 나열한 것으로이 자습서에서 자세히 알아볼 수 있습니다.

| 속성     | 설명                                                         |
| :------- | :----------------------------------------------------------- |
| alt      | 이미지를 표시 할 수 없을 때 이미지의 대체 텍스트를 지정합니다 |
| disabled | 입력 요소를 비활성화해야 함을 지정합니다                     |
| href     | 링크의 URL (웹 주소)을 지정합니다                            |
| id       | 요소의 고유 ID를 지정합니다                                  |
| src      | 이미지의 URL (웹 주소)을 지정합니다                          |
| style    | 요소의 인라인 CSS 스타일을 지정합니다                        |
| title    | 요소에 대한 추가 정보를 지정합니다 (툴팁으로 표시됨)         |

[HTML headings](./w3c/HTML_headings.md)


