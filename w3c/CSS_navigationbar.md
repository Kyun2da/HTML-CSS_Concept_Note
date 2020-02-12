# CSS Navigation Bar

## Navigation Bars

사용하기 쉬운 네비게이션을 가지는 것은 어떤 웹사이트던지 중요하다.

CSS를 사용하면 지루한 HTML 메뉴를 멋진 탐색 표시 줄로 변환 할 수 있다.

------

## Navigation Bar = List of Links

네비게이션 바는 표존 HTML을 기본으로써 요구한다.

우리의 예제에서 우리는 기초 HTML 리스트로부터 네비게이션 바를 만들 수있다.

네비게이션바는 일반적으로 링크의 리스트로 되어 있고 그래서 `<ul>`과  `<li>`엘리먼트를 사용한다.

### 예제

```html
<ul>
  <li><a href="default.asp">Home</a></li>
  <li><a href="news.asp">News</a></li>
  <li><a href="contact.asp">Contact</a></li>
  <li><a href="about.asp">About</a></li>
</ul>
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_basic_html)

이제 총알모양과 패딩과 마진을 리스트로부터 제거해보자

### 예제

```css
ul {
 list-style-type: none;
 margin: 0;
 padding: 0;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_basic_css)

예제는 다음과 같다.

- `list-style-type: none;` - 총알모양을 제거한다. 네비게이션 바는 리스트 마커가 필요하지 않기 때문이다.
-  `margin: 0;` 과 `padding: 0;` 을 기본 브라우저 세팅으로 부터 설정한다. 

위의 코드는 수직,수평 네비게이션바에 둘다 적용된다.

------

## Vertical Navigation Bar

수직 네비게이션바를 만들기 위해서는 너는 `<a>`엘리먼트를 리스트 안에서 스타일링 해야한다.

### 예제

```css
li a {
 display: block;
 width: 60px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_vertical)

예제는 다음과 같다.

- `display: block;` - 링크를 블록 요소로 표시하면 텍스트뿐만 아니라 전체 링크 영역을 클릭 할 수 있으며 너비 (및 원하는 경우 패딩, 여백, 높이 등)를 지정할 수 있게 해준다.
- `width: 60px;` - 블록 요소는 기본적으로 사용 가능한 전체 너비를 차지한다. 우리는 60 픽셀 너비를 지정했다.

`<ul>`의 너비를 설정하고 `<a>`의 너비를 제거 할 수도 있다. 블록 요소로 표시 될 때 사용 가능한 전체 너비를 차지하기 때문이다. 이전 예제와 동일한 결과가 생성된다.

### 예제

```css
ul {
 list-style-type: none;
 margin: 0;
 padding: 0;
 width: 60px;
}

li a {
 display: block;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_vertical2)

------

## Vertical Navigation Bar Examples

회색 배경색으로 기본 세로 탐색 모음을 만들고 사용자가 마우스를 링크 위로 이동할 때 링크의 배경색을 변경하는 예제를 만들어 보았다.

### 예제

```css
ul {
 list-style-type: none;
 margin: 0;
 padding: 0;
 width: 200px;
 background-color: #f1f1f1;
}

li a {
 display: block;
 color: #000;
 padding: 8px 16px;
 text-decoration: none;
}

/* Change the link color on hover */
li a:hover {
 background-color: #555;
 color: white;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_vertical_gray)

### Active/Current Navigation Link

현재 링크에 "active"클래스를 추가하여 사용자가 어느 페이지에 있는지 알릴수 있다.

### 예제

```css
.active {
 background-color: #4CAF50;
 color: white;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_vertical_active)

### Center Links & Add Borders

 `text-align:center` 를 추가해 텍스트를 가운데로 정렬할 수 있다.

border속성을 추가해 테두리의 색상을 지정해 테두리의 경계를 보여줄 수도 있다.

### 예제

```css
ul {
 border: 1px solid #555;
}

li {
 text-align: center;
 border-bottom: 1px solid #555;
}

li:last-child {
 border-bottom: none;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_vertical_borders)

### Full-height Fixed Vertical Navbar

고정 사이드 네비게이션바를 만든다.

### 예제

```css
ul {
 list-style-type: none;
 margin: 0;
 padding: 0;
 width: 25%;
 background-color: #f1f1f1;
 height: 100%; /* Full height */
 position: fixed; /* Make it stick, even on scroll */
 overflow: auto; /* Enable scrolling if the sidenav has too much content */
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_vertical_fixed)

**Note:** 이 예제는 모바일 기기에 적절하게 작동하지 않을 수도 있다.

------

## Horizontal Navigation Bar

가로 탐색 막대를 만드는 방법에는  **inline ** 또는 **float ** 항목을 사용하는 두 가지가 있다.

### Inline List Items

가로 방향 탐색 메뉴를 작성하는 한 가지 방법은 위의 "표준"코드 외에 <li> 요소를 인라인으로 지정하는 것이다.

### 예제

```css
li {
 display: inline;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal)

예제는 다음과 같다.

- `display: inline;` -  기본적으로 <li> 요소는 블록 요소다. 여기서는 각 목록 항목 전후에 줄 바꿈을 제거하여 한 줄에 표시한다.

### Floating List Items

가로 탐색 줄을 만드는 또 다른 방법은 `<li>`요소를 띄우고 탐색 링크의 레이아웃을 지정하는 것이다.

### 예제

```css
li {
 float: left;
}

a {
 display: block;
 padding: 8px;
 background-color: #dddddd;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal_float)

Example explained:

- `float: left;` - float를 사용하여 블록을 서로 띄우도록 만든다.
- `display: block;` -  링크를 블록 요소로 표시하면 텍스트뿐만 아니라 전체 링크 영역을 클릭 할 수 있으며 패딩 (및 원하는 경우 높이, 너비, 여백 등)을 지정할 수 있다.
- `padding: 8px;` - 블록 요소는 사용 가능한 전체 너비를 차지하므로 서로 옆에 띄울 수 없다. 따라서 패딩이 잘 보이도록 패딩을 지정해야한다.
- `background-color: #dddddd;` - 회색바탕색을 칠한다.

**Tip:** 전체 너비 배경색을 원하는 경우 각 <a> 요소 대신 <ul>에 배경색을 추가해야한다.

### 예제

```css
ul {
 background-color: #dddddd;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal_float2)

------

## Horizontal Navigation Bar Examples

배경색이 어두운 기본 가로 탐색 막대를 만들고 사용자가 마우스를 움직일 때 링크의 배경색을 변경하는 예제이다.

### 예제

```css
ul {
 list-style-type: none;
 margin: 0;
 padding: 0;
 overflow: hidden;
 background-color: #333;
}

li {
 float: left;
}

li a {
 display: block;
 color: white;
 text-align: center;
 padding: 14px 16px;
 text-decoration: none;
}

/* Change the link color to #111 (black) on hover */
li a:hover {
 background-color: #111;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal_black)

### Active/Current Navigation Link

현재 링크에 "active"클래스를 추가하여 사용자가 어느 페이지에 있는지 알려준다.

### 예제

```css
.active {
 background-color: #4CAF50;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal_black_active)

### Right-Align Links

목록 항목을 오른쪽 ( 'float : right;`)으로 플로팅하여 링크를 오른쪽 정렬한다.

### 예제

```html
<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li style="float:right"><a class="active" href="#about">About</a></li>
</ul>
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal_black_right)

### Border Dividers

테두리 경계를 만들려면`border-right` 속성을 <li>에 추가해야한다 :

### 예제

```css
/* Add a gray right border to all list items, except the last item (last-child) */
li {
 border-right: 1px solid #bbb;
}

li:last-child {
 border-right: none;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal_dividers)

### Fixed Navigation Bar

사용자가 페이지를 스크롤 할 때도 탐색 모음이 페이지의 맨 위나 맨 아래에 있도록한다.

### Fixed Top

```css
ul {
 position: fixed;
 top: 0;
 width: 100%;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal_black_fixed)

### Fixed Bottom

```css
ul {
 position: fixed;
 bottom: 0;
 width: 100%;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal_black_fixed2)

**Note:** 고정 포지션은 모바일에서는 작동하지 않을 수 있다.

### Gray Horizontal Navbar

얇은 회색 테두리가있는 회색 가로 탐색 막대의 예 :

### 예제

```css
ul {
 border: 1px solid #e7e7e7;
 background-color: #f3f3f3;
}

li a {
 color: #666;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal_gray)

### Sticky Navbar

`<ul>`에 `position : sticky;`를 추가하여 고정 탐색 모음을 만든다.


고정 요소는 스크롤 위치에 따라 상대 및 고정 사이를 전환한다. 주어진 오프셋 위치가 뷰포트에서 충족 될 때까지 상대적으로 배치 된 다음 위치에 고정된다 (예 : 위치 : 고정).

### 예제

```css
ul {
 position: -webkit-sticky; /* Safari */
 position: sticky;
 top: 0;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_sticky)

------

## More Examples

### Responsive Topnav

반응형 네비게이션 바이다.

![img](https://www.w3schools.com/css/navbar_responsive_hor.jpg)

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal_responsive)

### Responsive Sidenav

반응형 사이드 네비게이션 바다

![img](https://www.w3schools.com/css/navbar_responsive_ver.jpg)

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_vertical_responsive)

### Dropdown Navbar

네비게이션바의 드롭다운 메뉴를 구현한 것이다.

[Try iy Yourself ](https://www.w3schools.com/css/tryit.asp?filename=trycss_dropdown_navbar)

[CSS Dropdowns](./CSS_dropdowns.md)

