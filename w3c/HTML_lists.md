# HTML Lists

###  HTML List Example

### 순서 없는 리스트

- Item
- Item
- Item
- Item

### 순서 있는 리스트

1. First item
2. Second item
3. Third item
4. Fourth item

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_intro)

------

## 순서 없는 HTML List

순서 없는 리스트는 `<ul>`태그로 시작한다. 각각의 리스트 아이템은 `<li>`태그로 시작한다.

이 리스트 아이템들은 조그만 검정 동그라미로 마킹된다.

### 예제

```html
<ul>
 <li>Coffee</li>
 <li>Tea</li>
 <li>Milk</li>
</ul>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_unordered)

------

## 순서없는 HTML List - 리스트 마커

CSS `list-style-type` 속성은 리스트 아이템 마커의 스타일을 정의하는데 사용된다

| Value  | Description                              |
| :----- | :--------------------------------------- |
| disc   | 리스트 마커를 총알모양으로 한다(기본 값) |
| circle | 리스트 마커를 동그라미로 설정한다.       |
| square | 리스트 마커를 네모로 설정한다.           |
| none   | 리스트 마커를 없앤다                     |

### 예제 - Disc

```html
<ul style="list-style-type:disc;">
 <li>Coffee</li>
 <li>Tea</li>
 <li>Milk</li>
</ul>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_unordered_disc)

### 예제 - Circle

```html
<ul style="list-style-type:circle;">
 <li>Coffee</li>
 <li>Tea</li>
 <li>Milk</li>
</ul>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_unordered_circle)

### 예제 - Square

```html
<ul style="list-style-type:square;">
 <li>Coffee</li>
 <li>Tea</li>
 <li>Milk</li>
</ul>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_unordered_square)

### 예제 - None

```html
<ul style="list-style-type:none;">
 <li>Coffee</li>
 <li>Tea</li>
 <li>Milk</li>
</ul>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_unordered_none)



## 순서있는 HTML List

순서있는 아이템 리스트는 `<ol>`태그로 시작한다. 각각의 리스트 아이템은 `<li>`태그로 시작한다. 이 아이템 리스트는 디폴트로 숫자로 마킹되어 있다.

### 예제

```html
<ol>
 <li>Coffee</li>
 <li>Tea</li>
 <li>Milk</li>
</ol>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_ordered)

------

## 순서있는 HTML List - The Type Attribute

`<ol>`태그의  `<type>`속성은 리스트 아이템의 마커의 타입으로 정의된다.

| Type     | Description                                                  |
| :------- | :----------------------------------------------------------- |
| type="1" | The list items will be numbered with numbers (default)       |
| type="A" | The list items will be numbered with uppercase letters       |
| type="a" | The list items will be numbered with lowercase letters       |
| type="I" | The list items will be numbered with uppercase roman numbers |
| type="i" | The list items will be numbered with lowercase roman numbers |

### 숫자:

```html
<ol type="1">
 <li>Coffee</li>
 <li>Tea</li>
 <li>Milk</li>
</ol>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_ordered_numbers)

### 대문자:

```html
<ol type="A">
 <li>Coffee</li>
 <li>Tea</li>
 <li>Milk</li>
</ol>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_ordered_ucase)

### 소문자:

```html
<ol type="a">
 <li>Coffee</li>
 <li>Tea</li>
 <li>Milk</li>
</ol>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_ordered_lcase)

### 대문자 로마문자 :

```html
<ol type="I">
 <li>Coffee</li>
 <li>Tea</li>
 <li>Milk</li>
</ol>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_ordered_roman_ucase)

### 소문자 로마문자 :

```html
<ol type="i">
 <li>Coffee</li>
 <li>Tea</li>
 <li>Milk</li>
</ol>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_ordered_roman_lcase)

------

## HTML Description Lists

HTML은 또한 설명 리스트를 지지한다.

설명 리스트는 용어의 리스트이고 각각의 용어를 묘사한다.

`<dl>`태그는 설명 리스트를 정의하고 `<dt>`태그는 용어를 정의하고 `<dd>`태그는 각각의 용어를 묘사한다.

### 예제

```html
<dl>
 <dt>Coffee</dt>
 <dd>- black hot drink</dd>
 <dt>Milk</dt>
 <dd>- white cold drink</dd>
</dl>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_description)

------

## Nested HTML Lists

List can be nested (lists inside lists):

### 예제

```html
<ul>
	<li>Coffee</li>
	<li>Tea
		<ul>
			<li>Black tea</li>
			<li>Green tea</li>
            </ul>
    </li>
    <li>Milk</li>
</ul>

```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_nested)

**Note:** 리스트 아이템들은 다른 HTML 엘리먼트들, 이미지나 링크와 같은 새로운 리스트를 포함할 수 있다.

------

## Control List Counting

기본적으로 순서가 있는 리스트는 1로 시작한다.

만약 너가 특수한 숫자로 시작하기를 원한다면 너는 `start`속성을 사용하면 된다.

### 예제

```html
<ol start="50">
 <li>Coffee</li>
 <li>Tea</li>
 <li>Milk</li>
</ol>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_start)

------

## Horizontal List with CSS

HTML 리스트는 CSS에서 많은 다른 방법으로 스타일링 될 수 있다.

하나의 인기있는 방법은 네비게이션 메뉴를 만들기 위해 수평적으로 스타일하는 것이다. 

### 예제

```html
<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333333;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 16px;
  text-decoration: none;
}

li a:hover {
  background-color: #111111;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_lists_menu)

**Tip:** 너가 우리의 [CSS Tutorial](https://www.w3schools.com/css/default.asp)에 대해 더 배우고 싶다면 링크를 참조해라.

------

## Chapter Summary

- HTML `<ul>`엘리먼트는 순서없는 리스트를 사용할때 쓴다.
- `<list-style-type>`속성을 리스트 아이템 마커를 정의하는데에 사용해라
- `<ol>`엘리먼트를 순서가 있는 리스트를 정의하는데에 사용해라
- `type`속성을 숫자 타입을 정의하는데 사용해라
- `<li>`엘리먼트를 리스트 아이템을 정의하는데 사용해라
- `<dl>` 엘리먼트를 설명 리스트를 정의하는데 사용해라
- `<dt>`엘리먼트를 용어 설명을 정의하는데 사용해라
- `<dd>`엘리먼트를 용어리스트의 용어를 정의하는데 사용해라
- 리스트는 안의 리스트에 사용될 수 있다.
- 리스트 아이템은 다른 HTML 엘리먼트를 포함할 수 있다.
- CSS 속성 `float:left` 또는 `display:inline` 을 리스트를 수평적으로 표시할 때  사용해라

------



## HTML List Tags

| Tag    | Description               |
| :----- | :------------------------ |
| `<ul>` | 순서없는 리스트를 정의    |
| `<ol>` | 순서있는 리스트를 정의    |
| `<li>` | 리스트 아이템을 정의      |
| `<dl>` | 설명 리스트를 정의        |
| `<dt>` | 설명 리스트에 용어를 정의 |
| `<dd>` | 설명 리스트에 용어를 묘사 |

[HTML Blocks](./HTML_block.md)

