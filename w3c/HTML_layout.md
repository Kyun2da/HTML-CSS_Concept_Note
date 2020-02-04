# HTML Layouts

## HTML Layout Elements

웹사이트는 종종 많은 열의 내용들을 보여준다(뉴스나 잡지같은 레이아웃)

HTMl은 다양한 semantic 엘리먼트를 공급하고 그것을 웹페이지의 다른 부분으로 정의한다.

![HTML5 Semantic Elements](https://www.w3schools.com/html/img_sem_elements.gif)

`<header>` - 문서의 헤더부분을 정의한다.

`<nav>`- 네비게이션 링크를 위한 컨테이너를 정의한다.

`<section>` - 문서에 섹션을 정의한다.

`<article>` - 독립적인 기사를 정의한다.

`<aside>` - 사이드바와 같은 컨텐츠를 정의한다.

`<footer>` - 문서 또는 섹션의 바닥글을 정의한다.

`<details>` - 추가 세부사항을 정의한다.

`<summary>` -  `<details>` 엘리먼트의 제목을 정의한다.

------

## HTML Layout Techniques

다중 컬럼 레이아웃을 만드는 5가지의 다른 방법이 있다. 각각의 방법은 장점과 단점이 있다.

- HTML 테이블 (추천하지않음)
- CSS float 속성
- CSS flexbox
- CSS framework
- CSS grid

------

## 어떤것을 선택할까?

### HTML Tables

`<table>`엘리먼트는 레이아웃 툴로 디자인 될 수 없다.  `<table>`엘리먼트의 목적은 테이블형 데이터를 보여주는 것이다. 그래서 페이지 레이아웃을 위해 테이블을 사용하면 안된다. 그것들은 너의 코드에 혼잡함을 가져올 것이다. 그리고 그것이 몇달뒤에 너의 사이트가 다시 디자인 할 때의 어려움을 상상해 보면 안다.

**Tip:** 너의 페이지 레이아웃에는 테이블을 사용하지 말라!

------

### CSS 프레임워크

만약 너가 빠르게 너의 레이아웃을 만들고 싶으면 너는 프레임워크를 사용하면 된다.   [W3.CSS](https://www.w3schools.com/w3css/default.asp) 또는 [Bootstrap](https://www.w3schools.com/bootstrap/default.asp).

------

### CSS Floats

CSS float 속성을 사용하면서 웹 레이아웃을 만드는 것이 일반적인 일이다. Float는 배우기 쉽고 너는 단지 어떻게 float와 clear속성이 작동되는지만 기억하고 있으면 된다. **불이익** : floating 엘리먼트는 문서의 흐름에 묶여있고 그것은 융통적으로 해를 끼칠지도 모른다. 

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_layout_float)

------

### CSS Flexbox

Flexbox는 CSS에 새로운 레이아웃 모드이다.

flexbox의 사용은 엘리먼트가 페이지 레이아웃이 다른 화면 사이즈나 다른 디스플레이 기기들을 수용해야할 때 예측적으로 행동하는것을 보장한다. **불이익** : IE10이나 그보다 빠른 브라우저에서 동작을 하지 않는다. 

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_layout_flexbox)

------

### CSS Grid View

CSS 그리드 레이아웃 모듈은 그리드를 기반으로한 레이아웃 시스템이다. 행과 열이 있고 그것은 float나 positioning 없이 웹페이지를 더 쉽게 디자인할 수 있게 만들었다.

**불이익 :** IE나 EDGE15의 브라우저에서 작동하지 않는다.

[CSS Grid View](https://www.w3schools.com/css/css_rwd_grid.asp) 자세한것을 이 페이지를 참조하자.

[HTML Responsive Web Design](./HTML_responsive.md)