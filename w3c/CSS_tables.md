# CSS Tables

## Table 테두리

CSS에서 테이블 테두리를 특화시키기 위해서는 border 속성을 사용해라

아래의 예제는 table, th, td 엘리먼트를 검정 테두리를 만드는 예제이다.

### 예제

```css
table, th, td {
 border: 1px solid black;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_table_border)

위 예의 표에는 이중 테두리가 있다. 이는 테이블과 `<th>` 및 `<td>` 요소에 별도의 경계가 있기 때문이다.

------

## 테이블 테두리 축소

`border-collapse` 속성은 테이블 테두리를 단일 테두리로 축소할지 여부를 설정한다.

### 예제

```css
table {
 border-collapse: collapse;
}

table, th, td {
 border: 1px solid black;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_table_border-collapse)

테이블 주위에 테두리 만 원하면`<table>`에 `border` 속성 만 지정해라 :

### 예제

```css
table {
 border: 1px solid black;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_table_border2)

## 테이블 넓이와 높이

테이블의 너비와 높이는`width`와`height` 속성으로 정의된다.

아래 예제는 테이블 너비를 100 %로 설정하고 `<th>` 요소의 높이를 50px로 설정하는 예제이다.

### 예제

```css
table {
 width: 100%;
}

th {
 height: 50px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_table_width)

------

## 수평 정렬

`text-align` 속성은 <th> 또는 <td>에서 컨텐츠의 가로 정렬 (왼쪽, 오른쪽 또는 가운데)을 설정한다.

기본적으로 <th> 요소의 내용은 가운데 정렬되고 <td> 요소의 내용은 왼쪽 정렬됩니다.

다음 예제는 <th> 요소에서 텍스트를 왼쪽 정렬합니다.

### 예제

```css
th {
 text-align: left;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_table_align)

------

## 수직 정렬

`vertical-align` 속성은 <th> 또는 <td>에서 컨텐츠의 수직 정렬 (위, 아래 또는 중간)을 설정한다.

기본적으로 테이블 내용의 세로 정렬은 중간이다 (<th> 및 <td> 요소 모두).

다음 예제는 <td> 요소의 세로 텍스트 정렬을 bottom으로 설정한다.

### 예제

```css
td {
 height: 50px;
 vertical-align: bottom;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_table_vertical-align)

------

## 테이블 패딩

테두리와 표의 내용 사이의 간격을 제어하려면 <td> 및 <th> 요소의`padding` 속성을 사용해라

### 예제

```css
th, td {
 padding: 15px;
 text-align: left;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_table_padding)

------

## 수평 나누기

 `border-bottom` 속성을 추가해서 <th> 와 <td> 에대한 수평 나누기 를 제어할 수 있다.

### 예제

```css
th, td {
 border-bottom: 1px solid #ddd;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_table_border_divider)

------

## 강조할 수 있는 테이블

`:hover` 선택자를 사용하여 마우스 위에 행을 올려 테이블행을 강조할 수있다.

### 예제

```css
tr:hover {background-color: #f5f5f5;}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_table_hover)

------

## 줄무늬 테이블

| First Name | Last Name | Savings |
| :--------- | :-------- | :------ |
| Peter      | Griffin   | $100    |
| Lois       | Griffin   | $150    |
| Joe        | Swanson   | $300    |

줄무늬 테이블은 `nth-child()`선택자를 사용하여 모든 짝수나 홀수행 테이블에 배경색을 추가할 수 있다.

### 예제

```css
tr:nth-child(even) {background-color: #f2f2f2;}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_table_striped)

------

## 테이블 색상

아래 예제는 <th> 요소의 배경색과 텍스트 색을 지정하는 예제이다.

### 예제

```css
th {
 background-color: #4CAF50;
 color: white;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_table_color)

------

## Responsive Table

반응형 테이블은 내용을 모두 보여주고 싶은 테이블이 있을 경우 수평 스크롤 바를 이용하여 테이블을 만들 수 있다. 

| First Name | Last Name | Points | Points | Points | Points | Points | Points | Points | Points | Points | Points | Points | Points |
| :--------- | :-------- | :----- | :----- | :----- | :----- | :----- | :----- | :----- | :----- | :----- | :----- | :----- | :----- |
| Jill       | Smith     | 50     | 50     | 50     | 50     | 50     | 50     | 50     | 50     | 50     | 50     | 50     | 50     |
| Eve        | Jackson   | 94     | 94     | 94     | 94     | 94     | 94     | 94     | 94     | 94     | 94     | 94     | 94     |
| Adam       | Johnson   | 67     | 67     | 67     | 67     | 67     | 67     | 67     | 67     | 67     | 67     | 67     | 67     |

`<table>` 요소 주위에`overflow-x : auto`와 함께 컨테이너 요소 (예 : `<div>`)를 추가하여 반응 형으로 만듭니다.

### Example

```html
<div style="overflow-x:auto;">
	<table>... table content ...</table>
</div>
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_table_responsive)

## CSS Table Properties

| 속성                                                         | 설명                                                        |
| :----------------------------------------------------------- | :---------------------------------------------------------- |
| [border](https://www.w3schools.com/cssref/pr_border.asp)     | 한 번의 선언으로 모든 테두리 속성을 설정한다                |
| [border-collapse](https://www.w3schools.com/cssref/pr_border-collapse.asp) | 테이블 테두리를 축소할지 여부를 지정합니다                  |
| [border-spacing](https://www.w3schools.com/cssref/pr_border-spacing.asp) | 인접한 셀의 경계 사이의 거리를 지정한다                     |
| [caption-side](https://www.w3schools.com/cssref/pr_tab_caption-side.asp) | 테이블 캡션의 배치를 지정한다                               |
| [empty-cells](https://www.w3schools.com/cssref/pr_tab_empty-cells.asp) | 테이블의 빈 셀에 테두리 및 배경을 표시할지 여부를 지정한다. |
| [table-layout](https://www.w3schools.com/cssref/pr_tab_table-layout.asp) | 테이블에 사용될 레이아웃 알고리즘을 설정한다.               |

[CSS Layout](./CSS_layout.md)

