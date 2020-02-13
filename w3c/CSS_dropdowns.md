# CSS Dropdowns

CSS로 hover가능한 드롭다운을 만드는 예제이다.

------

## 기본적인 Dropdown

엘리먼트에 마우스를 올렸을 때 드롭다운 박스가 생성되게 하는 예제이다.

### 예제

```html
<style>
.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  padding: 12px 16px;
  z-index: 1;
}

.dropdown:hover .dropdown-content {
  display: block;
}
</style>

<div class="dropdown">
  <span>Mouse over me</span>
  <div class="dropdown-content">
    <p>Hello World!</p>
  </div>
</div>
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_dropdown_text)

### 예제 설명

**HTML)** 드롭다운 콘텐츠를 열기 위한 엘리먼트를 사용한다. `<span>` 이나 `<button>`과 같은 태그들을 쓸 수 있다.

컨테이너 요소 (예 : `<div>`)를 사용하여 드롭 다운 컨텐츠를 작성하고 그 안에 원하는 것을 추가할수 있다.

CSS로 드롭 다운 컨텐츠를 올바르게 배치하려면 요소 주위에 `<div>` 요소를 감싸면 된다.

**CSS)** `.dropdown` 클래스는 `position:relative`를 사용하고, 이것은 드롭다운 컨텐츠를 드롭다운 버튼 바로 아래에 배치하려는 경우에 사용한다.

.dropdown-content 클래스는 실제 드롭 다운 컨텐츠를 보유한다. 기본적으로 숨겨져 있으며 가리키면 표시된다 (아래 참조). 최소 너비는 160px로 설정되어 있다. 

------

## Dropdown Menu

사용자가 목록에서 옵션을 선택할 수있는 드롭 다운 메뉴를 만든다.

이 예제는 드롭 다운 상자 안에 링크를 추가하고 스타일 드롭 다운 버튼에 맞도록 스타일을 지정한다는 점을 제외하면 이전 예제와 비슷하다.

### 예제

```html
<style>
/* Style The Dropdown Button */
.dropbtn {
  background-color: #4CAF50;
  color: white;
  padding: 16px;
  font-size: 16px;
  border: none;
  cursor: pointer;
}

/* The container <div> - needed to position the dropdown content */
.dropdown {
  position: relative;
  display: inline-block;
}

/* Dropdown Content (Hidden by Default) */
.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

/* Links inside the dropdown */
.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}

/* Change color of dropdown links on hover */
.dropdown-content a:hover {background-color: #f1f1f1}

/* Show the dropdown menu on hover */
.dropdown:hover .dropdown-content {
  display: block;
}

/* Change the background color of the dropdown button when the dropdown content is shown */
.dropdown:hover .dropbtn {
  background-color: #3e8e41;
}
</style>

<div class="dropdown">
  <button class="dropbtn">Dropdown</button>
  <div class="dropdown-content">
    <a href="#">Link 1</a>
    <a href="#">Link 2</a>
    <a href="#">Link 3</a>
  </div>
</div>
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_dropdown_button)

------

## Right-aligned Dropdown Content

드롭 다운 메뉴를 왼쪽에서 오른쪽 대신 오른쪽에서 왼쪽으로 이동하려면`right : 0;`을 추가하면된다.

### 예제

```css
.dropdown-content {
 right: 0;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_dropdown_right)

------

## More Examples

### 드롭다운 이미지

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_dropdown_image)

### Dropdown Navbar

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_dropdown_navbar)



[CSS Image Gallery](./CSS_imagegallery.md)