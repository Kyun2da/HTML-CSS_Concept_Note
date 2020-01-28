#  How To Add CSS

브라우저가 스타일시트를 읽을 때, 이것은 스타일 시트에 있는 정보에 따라서 HTML 문서를 포맷팅합니다.

------

## CSS를 넣는 3가지 방법

스타일시트를 넣는 3가지 방법이 있습니다.

- 외부 CSS
- 내부 CSS
- 인라인 CSS

------

## 외부 CSS

외부스타일 시트를 쓸 때, 너는 하나의 파일을 변화시킴으로써 전체 웹사이트의 모습을 변화시킬 수 있습니다.

각각의 HTML 페이지는 외부 스타일 시트 파일에 대해 `<link>` 참조를 포함해야만 합니다.

### 예제

외부 스타일들은 `<link>` 엘리먼트 이내에 정의되고 HTML 페이지의 `<head>` 섹션안에 있어야만 합니다.

```html
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```



외부 스타일시트는 어떠한 텍스트 에디터로도 쓰여질 수 있고 .css 확장명으로 저장되어야 합니다.

외부 .css파일에는 어떠한 HTML 태그도 포함되어서는 안됩니다.

아래에 예제 "mystyle.css"가 있습니다.

### "mystyle.css"

```css
body {
 background-color: lightblue;
}

h1 {
 color: navy;
 margin-left: 20px;
}
```

**Note:** `margin-left: 20 px;` 와 같은 띄어쓰기를 사용하면 안됩니다. 반드시 `margin-left: 20px;` 과 같이 쓰세요.

### 내부 CSS

내부 스타일시트는 하나의 단일 HTML 페이지가 유니크 스타일이라면 사용될지도 모릅니다.

내부 스타일은 `<style>` 엘리먼트로 정의되어 있고 `<head> `섹션 안에 들어가야 합니다.

### 예제

내부 스타일은 `<style>`엘리먼트 안에 정의되어 있고 `<head>`섹션 안에 있어야 합니다.

```html
<!DOCTYPE html>
<html>
<head>
<style>
body {
 background-color: linen;
}

h1 {
 color: maroon;
 margin-left: 40px;
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

## 인라인 CSS

인라인 스타일은 하나의 엘리먼트를위해 독특한 스타일을 적용하기 위해 사용될지도 모릅니다.

인라인 스타일을 사용하기 위해서 관련있는 엘리먼트에 스타일 속성을 추가하세요. 이 스타일 속성은 어떠한 CSS 속성도 포함할 수 있습니다.

### 예제

인라인 스타일은 관련있는 엘리먼트의 속성을 스타일 안에 정의하면 됩니다.

```html
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
```



**Tip:** 인라인 스타일은 스타일시트의 많은 이점을 잃어버립니다(프레젠테이션과 같은 내용을 섞는 것). 이러한 방법을 나누어서 사용하세요.

------

## 다중 스타일 시트



`<h1>`엘리먼트와 같은 스타일로 외부 스타일시트를 쓴다고 생각해봅시다.

```css
h1 {
 color: navy;
}
```

그때 내부 스타일시트 또한 `<h1>`엘리먼트를 꾸며주고 있다고 생각해봅시다.

```css
h1 {
 color: orange;  
}
```



### 예제

만약 내부스타일이 외부스타일에 링크된 후에 정의된다면 h1 엘리먼트는 오렌지 색깔을 띌 것입니다.

```css
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
<style>
h1 {
 color: orange;
}
</style>
</head>
```



### 예제

그러나 링크가 그 다음에 온다면 h1의 색상은 네이비색을 띌 것입니다.

```css
<head>
<style>
h1 {
 color: orange;
}
</style>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```



## 계단식 순서(Cascading Order)

HTML 엘리먼트를위해 하나의 스타일보다 많은 스타일이 사용되고 있을때 어떤 스타일이 사용될 것인가?

페이지 안에있는 모든 스타일들은 계단식(Cascade) 속성을 가진다. 다음번호는 가장 높은 우선순위를 갖고 있다.

1. Inline style (inside an HTML element) HTML 엘리먼트 안의 인라인속성 
2. External and internal style sheets (in the head section) 헤드섹션안의 외부 혹은 내부 스타일시트
3. Browser default 브라우저 기본속성

따라서 인라인 스타일은 가장 높은 우선순위를 갖고 있으며 외부혹은 내부 스타일과 브라우저 스타일들은 그다음에 온다.

[CSS Colors](./CSS_colors.md)

