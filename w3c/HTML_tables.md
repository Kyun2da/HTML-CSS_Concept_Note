# HTML Tables

### HTML Table 예제

| Company                      | Contact          | Country |
| :--------------------------- | :--------------- | :------ |
| Alfreds Futterkiste          | Maria Anders     | Germany |
| Centro comercial Moctezuma   | Francisco Chang  | Mexico  |
| Ernst Handel                 | Roland Mendel    | Austria |
| Island Trading               | Helen Bennett    | UK      |
| Laughing Bacchus Winecellars | Yoshi Tannamuri  | Canada  |
| Magazzini Alimentari Riuniti | Giovanni Rovelli | Italy   |

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_table_intro)

------

## HTML Table 생성하기

HTML Table은 `<table>`태그로 정의됩니다.

각각의 테이블 행은 `<tr>`태그로 정의됩니다. 테이블 헤더는 `<th>`태그로 정의됩니다. 기본적으로 테이블 헤딩은 굵은 글씨이고 가운데 정렬입니다. 테이블 데이터와 셀들은 `<td>`태그로 정의됩니다.

### 예제

```html
<table style="width:100%">  
    <tr>  
        <th>Firstname</th>    
        <th>Lastname</th>    
        <th>Age</th>  
    </tr>  
    <tr>    
        <td>Jill</td>    
        <td>Smith</td>    
        <td>50</td>  
    </tr>  
    <tr>    
        <td>Eve</td>    
        <td>Jackson</td>    
        <td>94</td>  
    </tr>
</table>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_table)

**Note:** `<td>`엘리먼트는 테이블의 데이터 컨테이너 입니다. 그들은 HTML 엘리먼트의 모든 정렬을 포함할 수 있습니다.



## HTML Table - Adding a Border

만약 너가 테이블의 테두리를 특정하지 않는다면 그것은 테두리 없이 보여질 것입니다.

테두리는 CSS 테두리 속성을 사용하여 적용됩니다.

### 예제

```css
table, th, td {
 border: 1px solid black;
}
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_table_border)

테이블과 테이블 셀 둘다 테두리를 정의할 수 있다는 것을 기억해라

------

## HTML Table - Collapsed Borders

만약 너가 하나의 테두리를 없애고 싶으면 CSS `border-collapse`속성을 쓰면 된다.

### 예제

```css
table, th, td {
 border: 1px solid black;
 border-collapse: collapse;
}
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_table_collapse)

------

## HTML Table - Adding Cell Padding

Cell 패딩은 셀 내용과 그것의 테두리 사이의 공간을 정의합니다.

만약 패딩이 정의되지 않는 다면 테이블 셀은 패딩 없이 셀을 보여줄 것입니다.

패딩을 두기위해서는 `padding`속성을 사용해야만 합니다.

### 예제

```css
th, td {
 padding: 15px;
}
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_table_cellpadding)

------

## HTML Table - Left-align Headings

기본적으로 테이블 헤딩은 굵은 글씨와 중앙 정렬이다.

테이블 헤딩을 왼쪽 정렬하기 위해서는 CSS의 `text-align`속성을 사용해라

### 예제

```css
th {
 text-align: left;
}
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_table_headings_left)

------

## HTML Table - Adding Border Spacing

테두리 공간은 셀 사이의 공간에 특화되어있다.

테이블의 공간 테두리를 정하기 위해서는 CSS `border-spacing`속성을 사용해야한다.

### 예제

```css
table {
 border-spacing: 5px;
}
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_table_cellspacing)

**Note:** 만약 테이블이 분리된 테두리를 가지고있지않다면 border-spacing은 효과가 없다

------

## HTML Table - Cells that Span Many Columns

cell span을 하나의 열이상 만들려고 한다면 `colspan` 속성을 사용해라

### 예제

```html
<table style="width:100%">  
  	<tr>
  	  <th>Name</th>    
      <th colspan="2">Telephone</th>  
    </tr>  
    <tr>    
        <td>Bill Gates</td>
        <td>55577854</td>
        <td>55577855</td>
    </tr>
</table
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_table_colspan)

------

## HTML Table - Cells that Span Many Rows

하나의 행보다 더많은 cell을 span한다면 `rowspan`속성을 사용해라

### 예제

```html
<table style="width:100%">
	<tr>    
    	<th>Name:</th>    
    	<td>Bill Gates</td>  
	</tr>  
    <tr> 				
        <th rowspan="2">Telephone</th>
        <td>55577854</td>
    </tr>
    <tr>    
        <td>55577855</td>
    </tr>
</table>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_table_rowspan)

------

## HTML Table - Adding a Caption

테이블에 캡션을 넣고싶다면 `<caption>`태그를 사용해라

### 예제

```html
<table style="width:100%">
    <caption>Monthly savings</caption>
    <tr>
        <th>Month</th>  
    	<th>Savings</th>
  	</tr>
    <tr>
        <td>January</td>
        <td>$100</td>
    </tr>
    <tr>
        <td>February</td>
        <td>$50</td> 
    </tr>
</table>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_tables2)

**Note:** `<caption>`태그는 `<table>`태그 후에 즉시 삽입되어야만 한다.

------

## A Special Style for One Table

테이블에 특수한 스타일을 정의하기 위해서는 테이블에 `<id>`속성을 추가해야만 한다.

### 예제

```html
<table id="t01">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th>
        <th>Age</th>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
</table>
```



### 이제 너는 이테이블에 특수한 스타일을 넣을 수 있다.

```css
table#t01 {
 width: 100%;
 background-color: #f1f1c1;
}
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_table_id1)

### 더많은 스타일을 추가해라

```css
table#t01 tr:nth-child(even) {
 background-color: #eee;
}
table#t01 tr:nth-child(odd) {
 background-color: #fff;
}
table#t01 th {
 color: white;
 background-color: black;
}
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_table_id2)

------

## 챕터 요약

- 테이블을 정의하기 위해서는 `<table>`원소를 사용해라
- 테이블 행을 정의하기 위해서는 `<tr>`태그를 사용해라
- 태이블 데이터를 정의하기 위해서는 `<td>`태그를 사용해라
- 테이블 헤딩을 정의하기 위해서는 `<th>`태그를 사용해라
- 테이블에 캡션을 적용하기 위해서는 `<caption>`태그를 사용해라
- 테두리를 정의하기 위해서는 CSS  `<border>`속성을 사용해라
- cell 경계를 바꾸기 위해서는 CSS   `border-collapse`  속성을 사용해라
- 셀에 패딩을 추가하고 싶으면 CSS   `padding` 속성을 사용해라
- 셀 텍스트 정렬을 사용하고 싶다면 CSS   `text-align` 속성을 사용해라
- 셀 사이에 공간을 두고 싶다면 CSS  `border-spacing`  속성을 사용해라
- 셀의 많은 열들을 합치고 싶으면  `colspan`  속성을 사용해라
- 셀의 많은 행들을 합치고 싶으면 `rowspan`  속성을 사용해라
- 하나의 테이블의 독특한 정의를 하고싶다면  `id` 속성을 사용해라

------



## HTML Table Tags

| 태그         | 설명                                                         |
| :----------- | :----------------------------------------------------------- |
| `<table>`    | 테이블을 정의한다                                            |
| `<th>`       | 테이블 안에 헤더 셀을 정의한다.                              |
| `<tr>`       | 테이블 안에 행을 정의한다.                                   |
| `<td>`       | 테이블 안에 셀들을 정의한다.                                 |
| `<caption>`  | 테이블 캡션을 정의한다.                                      |
| `<colgroup>` | 테이블 포맷팅에서 많은 열을 하나의 그룹으로 만든다           |
| `<col>`      | <colgroup> 엘리먼트 이내에 각각의 열들의 속성을 특수화 한다. |
| `<thead>`    | 테이블안의 내용을 헤더로 그룹화한다.                         |
| `<tbody>`    | 테이블 안에 내용을 body로 그룹화한다.                        |
| `<tfoot>`    | 테이블 안의 내용을 footer로 그룹화한다.                      |

[HTML Lists](./HTML_lists.md)

