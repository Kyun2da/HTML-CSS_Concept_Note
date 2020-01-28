## CSS 선택자

CSS 선택자는 HTML 엘리먼트들을 너가 원하는 색상으로 하고싶을때 선택하는 것이다.

우리는 CSS 선택자를 5개의 카테고리로 나눌 수 있다.

- 간단한 선택자(이름, 아이디, 클래스 등으로 된 선택자들)
- 혼합선택자(서로의 사이이 관계에 기초해있는 선택자들)
- pseudo-class선택자(특정한상태에 기초한 선택자들)
- Pseudo-elements 선택자 (엘리먼트의 한 부분의 스타일을 선택하는것)
- 속성 선택자 (속성이나 속성값에 기초한 엘리먼트들을 선택하는것)

이 페이지는 가장 기초적인 CSS 선택자들을 설명할 것이다.



## CSS 엘리먼트 선택자

엘리먼트 선택자는 엘리먼트 이름을 토대로 HTML 엘리먼트를 선택한다.

### 예제

아래에 모든 `<p>`엘리먼트들은 중앙정렬되고 빨간색을 갖는다.

```css
p {
  text-align: center;
  color: red;
}
```



## The CSS id Selector

The id selector uses the id attribute of an HTML element to select a specific element.

The id of an element is unique within a page, so the id selector is used to select one unique element!

To select an element with a specific id, write a hash (#) character, followed by the id of the element.

### Example

The CSS rule below will be applied to the HTML element with id="para1": 

```css
#para1 {
 text-align: center;
 color: red;
}
```



## CSS id 선택자

이 id 선택자는 HTML 엘리먼트의 id를 통해서 html 엘리먼트를 선택한다.

엘리먼트의 아이디는 페이지 안에있는 하나의 유니크한 아이디이다. 따라서 아이디 선택자는 하나의 유니크한 엘리먼트를 선택하는데 사용된다.

특수한 아이디를 가진 엘리먼트를 선택하는 것은 #문자를 이용해 아이디를 선택한다.

### 예제

아래 HTML 엘리먼트에 적용될 CSS 규약은 id="para1"이라는 것이다.

```css
#para1 {
 text-align: center;
 color: red;
}
```



**Note:** 아이디는 숫자로 시작해서는 안된다!



## The CSS 클래스 선택자

특수한 클래스 속성을 가진 HTML 엘리먼트를 클래스 선택자가 선택한다.

특수한 클래스를 가진 엘리먼트를 선택하기 위해서 .문자를 써서 클래스를 사용한다.

### 예제

이 예제에서 class="center" 클래스를 가진 모든 HTML 엘리먼트는 빨강색과 중앙 정렬이 될 것이다.

```css
.center {
 text-align: center;
 color: red;
}
```



너는 클래스에 영향을 미치는 엘리먼트를 단 하나의 엘리먼트로 한정할 수 있다.

### 예제

아래 예제는 p태그의 클래스 center 만 영향을 미치게하는 예제이다.

```css
p.center {
 text-align: center;
 color: red;
}
```



HTML 요소는 둘 이상의 클래스를 참조 할 수도 있다

### 예제

`<p>` 엘리먼트에 center 클래스와 large 클래스를 넣은 예제이다.

```css
<p class="center large">This paragraph refers to two classes.</p>
```



**Note:** 클래스 이름은 숫자로 시작할 수 없다.

------

## The CSS Universal 선택자

유니버셜 선택자는 (*) 페이지에있는 모든 선택자를 선택한다.

### 예제

아래 CSS 규칙은 페이지에 모든 엘리먼트에 영향을 끼친다.

```css
* {
 text-align: center;
 color: blue;
}
```



------

## The CSS 그룹 선택자

그룹 선택자는 같은 스타일 정의의 HTML엘리먼트를 선택한다.

아래의 엘리먼트들은 모두 같은 스타일을 갖고 있다.

```css
h1 {
 text-align: center;
 color: red;
}

h2 {
 text-align: center;
 color: red;
}

p {
 text-align: center;
 color: red;
}
```

아래의 예제는 위의 예제를 단순화 시킬 수 있어 가독성이 좋다.

### 예제 

```css
h1, h2, p {
 text-align: center;
 color: red;
}
```



## 모든 CSS 선택자

| 선택자                                                       | 예         | 설명                              |
| :----------------------------------------------------------- | :--------- | :-------------------------------- |
| [.*class*](https://www.w3schools.com/cssref/sel_class.asp)   | .intro     | class="intro"를 선택한다.         |
| [#*id*](https://www.w3schools.com/cssref/sel_id.asp)         | #firstname | id="firstname"을 선택한다.        |
| [*](https://www.w3schools.com/cssref/sel_all.asp)            | *          | 모든 엘리먼트를 선택한다.         |
| *[element](https://www.w3schools.com/cssref/sel_element.asp)* | p          | 모든 <p> 엘리먼트를 선택한다.     |
| *[element,element,..](https://www.w3schools.com/cssref/sel_element_comma.asp)* | div, p     | 모든 div와 p 엘리먼트를 선택한다. |

[How To Add Css](./CSS_howtoaddcss.md)