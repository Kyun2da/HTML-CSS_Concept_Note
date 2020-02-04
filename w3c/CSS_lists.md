# CSS Lists

## 순서없는 리스트 :

- Coffee
- Tea
- Coca Cola

- Coffee
- Tea
- Coca Cola

## 순서있는 리스트 :

1. Coffee
2. Tea
3. Coca Cola

1. Coffee
2. Tea
3. Coca Cola

------

## HTML 리스트와 CSS 리스트 속성

HTML에서 리스트의 두가지 타입이 있다.

- 순서없는 리스트 (<ul>) - 순서없는 리스트 아이템은 총알모양으로 마킹되어있다.
- 순서있는 리스트 (<ol>) - 순서있는 리스트 아이템은 숫자나 글자로 마킹되어 있다.

CSS리스트 속성은 너에게 다음과 같은 것을 허용한다:

- 순서있는 리스트는 다른 리스트 아이템 마킹을 세팅한다.
- 순서없는 리스트에 대해 다른 목록 항목 마커 설정
- 이미지를 목록 항목 마커로 설정
- 리스트 및 리스트 항목에 배경색 추가

------

## 다른 리스트 아이템 마커

 `list-style-type` 속성은 리스트 아이템 마커의 타입을 정의한다.

다음과 같은 예제는 리스트 아이템 마커의 가능한 목록을 보여준다.

### 예제

```css
ul.a {
 list-style-type: circle;
}

ul.b {
 list-style-type: square;
}

ol.c {
 list-style-type: upper-roman;
}

ol.d {
 list-style-type: lower-alpha;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_list-style-type_ex)

## 리스트 아이템마커를 이미지로 사용하기

 `list-style-image` 속성은 아이템 마커를 이미지로 사용할 수 있도록 한다.

### 예제

```css
ul {
 list-style-image: url('sqpurple.gif');
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_list-style-image)

------

## 리스트 아이템 마커 위치

 `list-style-position` 속성은 리스트 아이템 마커의 위치에 특화되어 있는 속성이다.

"list-style-position: outside;" 는 글 머리 기호가 목록 항목 외부에 있음을 의미한다. 목록 항목의 각 줄의 시작은 세로로 정렬된다. 이것이 기본값이다.

"list-style-position: inside;" 는 글머리 기호가 항목 안에 있음을 의미한다. 목록 항목의 일부이므로 텍스트의 일부가되고 시작시 텍스트를 푸시한다.

### 예제

``` css
ul.a {
 list-style-position: outside;
}

ul.b {
 list-style-position: inside;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_list-style-position)

------

## 기본값을 제거하기

 `list-style-type:none` 속성은 마커를 제거하는데 사용된다. 리스트는 디폴트 마진과 패딩을 갖고있다. 이것을 제거하면 마진은0이되고 패딩도 0이된다. 

### 예제

```css
ul {
 list-style-type: none;
 margin: 0;
 padding: 0;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_list-style_none)

------

## List - Shorthand property

 `list-style` 속성은 짧게 쓰는 속성이다 이것은 모든 리스트 속성을 하나의 선언으로 쓸 수 있다

### 예제

```css
ul {
 list-style: square inside url("sqpurple.gif");
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_list-style)

짧게 속성을 쓸때, 속성값의 순서는 다음과 같다

- `list-style-type` (목록 스타일 이미지가 지정된 경우, 어떤 이유로 이미지를 표시 할 수없는 경우이 특성의 값이 표시된다)
- `list-style-position` (목록 항목 마커가 컨텐츠 플로우 내부 또는 외부에 표시되어야하는지 지정)
- `list-style-image` (이미지를 목록 항목 마커로 지정)

위의 속성 값 중 하나가 누락 된 경우 누락된 속성의 기본값이 있으면 삽입된다.

------

## Styling List With Colors

또한 좀 더 흥미롭게 보이도록 색상으로 목록 스타일을 지정할 수도 있습니다.

`<ol>`또는 `<ul>` 태그에 추가 된 것은 전체 목록에 영향을 미치며 `<li>`태그에 추가 된 속성은 개별 목록 항목에 영향을 미친다.

### 예제

```css
ol {
 background: #ff9999;
 padding: 20px;
}

ul {
 background: #3399ff;
 padding: 20px;
}

ol li {
 background: #ffe5e5;
 padding: 5px;
 margin-left: 35px;
}

ul li {
 background: #cce5ff;
 margin: 5px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_list-style_colors)

------

## All CSS List Properties

| 속성                                                         | 설명                                             |
| :----------------------------------------------------------- | :----------------------------------------------- |
| [list-style](https://www.w3schools.com/cssref/pr_list-style.asp) | 한 선언에서 목록의 모든 속성을 설정한다          |
| [list-style-image](https://www.w3schools.com/cssref/pr_list-style-image.asp) | 이미지를 목록 항목 마커로 지정                   |
| [list-style-position](https://www.w3schools.com/cssref/pr_list-style-position.asp) | 목록 항목 마커 (글 머리 기호)의 위치를 지정한다. |
| [list-style-type](https://www.w3schools.com/cssref/pr_list-style-type.asp) | 목록 항목 마커의 유형을 지정한다.                |

[CSS Tables](./CSS_tables.md)