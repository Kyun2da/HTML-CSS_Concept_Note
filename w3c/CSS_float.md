# CSS Layout - float and clear

The CSS `float`  속성은 어떻게 엘리먼트가 떠있을지를 정한다.

CSS clear 속성은 지워진 요소 옆과 어느쪽에 어떤 요소를 띄울 수 있는지 지정한다.

------

## The float Property

`float` 속성은 콘텐츠를 배치하고 형식을 지정하는 데 사용된다 (예 : 이미지를 컨테이너의 텍스트 왼쪽에 띄웁니다.

`float` 속성은 다음 값 중 하나를 가질 수 있다.

- left-요소가 컨테이너의 왼쪽에 뜬다
- right-요소가 컨테이너의 오른쪽에 뜬다
- none-요소가 플로팅되지 않는다 (텍스트에서 발생하는 위치에 표시됩니다). 이것이 기본값입니다
- inherit-요소는 부모의 float 값을 상속받는다.

가장 간단한 사용법으로,`float` 속성을 사용하여 이미지 주위에 텍스트를 감쌀 수 있다.

------

## Example - float: right;

### 예제

```css
img {
 float: right;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_float)

------

## Example - float: left;

### 예제

```css
img {
 float: left;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_float2)

------

## Example - No float

### 예제

```css
img {
 float: none;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_float_none)

------

## The clear Property

'clear'속성은 지워진 요소 옆에 어떤 요소가 떠 다닐 수 있는지 지정한다.

`clear` 속성은 다음 값 중 하나를 가질 수 있습니다.

- none-양쪽에 플로팅 요소를 허용합니다. 이것이 기본값입니다
- 왼쪽-왼쪽에 플로팅 요소가 허용되지 않습니다
- 오른쪽-오른쪽에 부동 요소가 허용되지 않습니다
- 둘 다-왼쪽 또는 오른쪽에 부동 요소가 허용되지 않습니다
- inherit-요소는 부모의 명확한 가치를 상속

`clear` 속성을 사용하는 가장 일반적인 방법은 요소에`float` 속성을 사용한 후에입니다.

플로트를 지울 때는 클리어와 플로트를 일치시켜야합니다. 요소가 왼쪽에 떠 있으면 왼쪽으로 지워야합니다. 플로팅 된 요소는 계속 플로팅되지만 삭제 된 요소는 웹 페이지 아래에 나타납니다.

다음 예제에서는 부동 소수점을 왼쪽으로 지 웁니다. div의 왼쪽에 부동 요소가 허용되지 않음을 의미합니다.

### 예제

```css
div {
 clear: left;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_clear)

------

## The clearfix Hack

요소가 요소를 포함하는 요소보다 키가 크고 부동 상태 인 경우 컨테이너 외부로 "오버 플로우"된다.

### Without Clearfix

![img](https://www.w3schools.com/howto/clearfix_prob.jpg)

### With Clearfix

![img](https://www.w3schools.com/howto/clearfix_solution.jpg)

그런 다음 포함 요소에`overflow : auto;`를 추가하여이 문제를 해결할 수 있다.

### 예제

```css
.clearfix {
 overflow: auto;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_clearfix)

`overflow : auto` clearfix는 여백과 패딩을 제어 할 수있는 한 잘 작동한다 (스크롤바가 표시 될 수도 있음). 그러나 **새롭고 현대적인 clearfix hack **은 사용하기에 안전하며 다음 코드는 대부분의 웹 페이지에 사용된다.

### 예제

```css
.clearfix::after {
 content: "";
 clear: both;
 display: table;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_clearfix2)

You will learn more about the `::after` pseudo-element in a later chapter.

------

## Grid of Boxes / Equal Width Boxes

`float` 속성을 사용하면 내용 상자를 나란히 띄울 수 있다.

### 예제

```css
* {
 box-sizing: border-box;
}

.box {
 float: left;
 width: 33.33%; /* three boxes (use 25% for four, and 50% for two, etc) */
 padding: 50px; /* if you want space between the images */
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_float_boxes)

**box-sizing 이란 무엇인가? **

3 개의 부동 상자를 나란히 쉽게 만들 수 있다. 그러나 각 상자의 너비를 늘리는 항목 (예 : 패딩 또는 테두리)을 추가하면 상자가 깨진다. 'box-sizing'속성을 사용하면 상자의 전체 너비 (및 높이)에 패딩과 테두리를 포함하여 패딩이 상자 안에 유지되고 끊어지지 않도록 할 수 있다.

------

## Images Side By Side

### 예제

```css
.img-container {
 float: left;
 width: 33.33%; /* three containers (use 25% for four, and 50% for two, etc) */
 padding: 5px; /* if you want space between the images */
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_float_images_side)

------

## Equal Height Boxes

이전 예제에서는 상자를 같은 너비로 나란히 플로팅하는 방법을 배웠다. 그러나 같은 높이의 부동 상자를 만드는 것은 쉽지 않다. 그러나 빠른 수정은 아래 예와 같이 고정 된 높이를 설정하는 것이다.

### 예제

```css
.box {
 height: 500px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_float_boxes_height)

**그러나 ** 이것은 매우 유연하지 않다. 상자에 항상 같은 양의 내용이 포함되도록 보장 할 수 있다면 괜찮다. 그러나 여러 번 내용이 동일하지 않다. 위의 예를 휴대폰에서 시도하면 두 번째 상자의 내용이 상자 외부에 표시된다. CSS3 Flexbox가 유용한 이유는 가장 긴 상자만큼 상자를 자동으로 늘릴 수 있기 때문이다.

### 예제

**Flexbox **를 사용하여 유연한 상자 만들기 :

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_float_boxes_flex)

------

## Navigation Menu

하이퍼 링크 목록과 함께 `float`을 사용하여 가로 메뉴를 만든다.

### 예제

- [Home](javascript:void(0))
- [News](javascript:void(0))
- [Contact](javascript:void(0))
- [About](javascript:void(0))

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_float5)

------

## Web Layout Example

`float`속성을 사용하여 전체 웹 레이아웃을 수행하는 것도 일반적입니다.


### 예제

```css
.header, .footer {
 background-color: grey;
 color: white;
 padding: 15px;
}

.column {
 float: left;
 padding: 15px;
}

.clearfix::after {
 content: "";
 clear: both;
 display: table;
}

.menu {
 width: 25%;
}

.content {
 width: 75%;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_cols)

------

## All CSS Float Properties

| 속성                                                         | 설명                                                         |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [box-sizing](https://www.w3schools.com/cssref/css3_pr_box-sizing.asp) | 요소의 너비와 높이가 계산되는 방식을 정의합니다. 패딩과 테두리를 포함해야하는지 여부 |
| [clear](https://www.w3schools.com/cssref/pr_class_clear.asp) | 지워진 요소 옆에 어떤 요소가 떠 다닐 수 있는지 지정합니다.   |
| [float](https://www.w3schools.com/cssref/pr_class_float.asp) | 요소가 어떻게 떠야 하는지를 지정                             |
| [overflow](https://www.w3schools.com/cssref/pr_pos_overflow.asp) | 내용이 요소 상자에 넘칠 경우 어떻게되는지 지정               |
| [overflow-x](https://www.w3schools.com/cssref/css3_pr_overflow-x.asp) | 내용이 요소의 내용 영역에 넘칠 경우 내용의 왼쪽 / 오른쪽 가장자리로 수행 할 작업을 지정합니다. |
| [overflow-y](https://www.w3schools.com/cssref/css3_pr_overflow-y.asp) | 내용이 요소의 내용 영역에 넘칠 경우 내용의 위쪽 / 아래쪽 가장자리로 수행 할 작업을 지정합니다. |

[CSS inline-block](./CSS_inlineblock.md)