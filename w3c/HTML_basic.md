# HTML 기본 예제들

이번 챕터에서 당신이 배우지않은 태그들을 사용한다고 해도 걱정하지 마세요.

당신은 다음 챕터에서 그것들에 관해 배울겁니다.

## HTML 문서

모든 HTML 문서들은 문서타입 선언으로 시작해야합니다 : `<!DOCTYPE html>`.

HTML 문서 그것자체는 `<html>`로 시작하고 `</html>`로 끝납니다.

HTML 문서의 볼 수 있는 부분은 `<body>` 와 `</body>` 사이에 들어갑니다.

### 예시

```html
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```

## HTML Headings(헤딩)

HTML 헤딩들은 `<h1>`부터 `<h6>` 태그로 정의됩니다.

`<h1>` 은 가장 중요한 헤딩으로 정의됩니다. `<h6>`은 가장 덜 중요한 헤딩으로 정의됩니다.

### 예시

```html
<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<h3>This is heading 3</h3>
```

## HTML Links(링크)

HTML링크는 `<a>` 태그로 정의됩니다.

### 예시

```html
<a href="https://www.w3schools.com">This is a link</a>
```

이링크의 목적지는 **href**라는 속성안에 씁니다.

속성들은 HTML 원소들에 관해 추가적인 정보를 공급할때 사용합니다.

당신은 이 후의 챕터들에서 이와 같은 속성들에 대해 더 배우게 될 것 입니다.

## HTML Images(이미지)

HTML 이미지들은 `<img>` 태그로 정의됩니다.

소스파일은 src, 대체 택스트는 alt, width와 height 등의 속성이 제공됩니다.

### 예시

```html
<img src="w3schools.jpg" alt="W3Schools.com" width="104" height="142">
```

## HTML Buttons(버튼)

HTML 버튼은 `<button>` 태그로 정의됩니다.

### 예시

```html
<button>Click me</button>
```

## HTML Lists

HTML 리스트들은 순서가 있는 리스트와 순서가 없는 리스트가 있습니다.

순서가 있는 리스트들은 `<ol></ol>`을 쓰고 순서가 없는 리스트들은 `<ul></ul>`태그를 씁니다. 그리고 그안의 리스트들은 `<li></li>`로 감싸집니다.

### Example

```html
<ul>  
    <li>Coffee</li>  
    <li>Tea</li>  
    <li>Milk</li>
</ul>
<ol>  
    <li>Coffee</li>  
    <li>Tea</li>  
    <li>Milk</li>
</ol>
```

[HTML 원소들로가기](./w3c/HTML_elements.md)

