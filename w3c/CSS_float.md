# CSS Layout - float and clear

CSS `float`속성은 어떻게 엘리먼트가 떠있어야할지를 정한다.

CSS `clear` 속성은 지워진 엘리먼트 옆과 어느쪽에 어떤 엘리먼트를 띄울 수 있는지 지정합니다.

------

## The float Property

float 속성은 콘텐츠를 배치하고 형식을 지정하는 데 사용된다 (예 : 이미지를 컨테이너의 텍스트 왼쪽에 띄운다.

`float`속성은 다음과 같은 값들 중 하나를 가질 수 있다.

- left - 그것의 컨테이너를 왼쪽에 띄운다.
- right -  그것의 컨테이너를 오른쪽에 띄운다.
- none - 요소가 플로팅되지 않는다. (텍스트에서 발생하는 위치에만 표시됨). 이것이 기본값
- inherit - 요소는 부모의 float 값을 상속받는다.

가장 간단한 사용법으로,`float` 속성을 사용하여 이미지 주위에 텍스트를 감쌀 수 있다.

------

## 예제 - float: right;

다음 예제는 이미지가 텍스트에서 **오른쪽 **으로 부동되도록 지정한다.

### 예제

```css
img {
 float: right;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_float)

------

## 예제 - float: left;

다음 예제는 이미지가 텍스트에서 **왼쪽 **으로 부동되도록 지정한다.

### 예제

```css
img {
 float: left;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_float2)

------

## 예제 - No float

다음 예제에서는 이미지가 텍스트에서 발생하는 위치에 표시된다 (float : none;).

### 예제

```css
img {
 float: none;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_float_none)

------

## The clear Property

`clear` 속성은 지워진 요소 옆에 어떤 요소가 떠 다닐 수 있는지 지정한다.

`clear` 속성은 다음 값 중 하나를 가질 수 있다.

- none - 양쪽에 플로팅 요소를 허용합니다. 이것이 기본값이다.
- left - 왼쪽에 플로팅 요소가 허용되지 않는다
- right- 오른쪽에 플로팅 요소가 허용되지 않는다
- both - 양쪽에 플로팅 요소가 허용되지 않는다
- inherit - 부모의 clear 값을 상속받는다.

`clear` 속성을 사용하는 가장 일반적인 방법은 요소에`float` 속성을 사용한 후에다.

플로트를 지울 때는 클리어와 플로트를 일치시켜야한다. 요소가 왼쪽에 떠 있으면 왼쪽으로 지워야한다. 플로팅 된 요소는 계속 플로팅되지만 클리어 된 요소는 웹 페이지 아래에 나타납니다.

다음 예제에서는 부동 소수점을 왼쪽으로 지운다. div의 왼쪽에 부동 요소가 허용되지 않음을 의미한다.

### 예제

```css
div {
 clear: left;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_clear)

------

<iframe id="google_ads_iframe_/22152718/sws-hb//w3schools.com//mid_content_0" title="3rd party ad content" name="google_ads_iframe_/22152718/sws-hb//w3schools.com//mid_content_0" width="728" height="90" scrolling="no" marginwidth="0" marginheight="0" frameborder="0" srcdoc="" data-google-container-id="4" data-load-complete="true" style="box-sizing: inherit; border: 0px; vertical-align: bottom;"></iframe>

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

'오버플로 : 자동'clearfix는 여백과 패딩을 제어 할 수있는 한 잘 작동한다 (스크롤바가 표시 될 수도 있음). **새롭고 현대적인 clearfix hack **은 사용하기에 안전하며 다음 코드는 대부분의 웹 페이지에 사용됩니다.

### 예제

```css
.clearfix::after {
 content: "";
 clear: both;
 display: table;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_clearfix2)

다음 장에서`:: after` 의사 요소에 대해 더 배울 것입니다.

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

**What is box-sizing?**

3 개의 부동 상자를 나란히 쉽게 만들 수 있다. 그러나 각 상자의 너비를 늘리는 항목 (예 : 패딩 또는 테두리)을 추가하면 상자가 깨진다. 'box-sizing'속성을 사용하면 상자의 전체 너비 (및 높이)에 패딩과 테두리를 포함하여 패딩이 상자 안에 유지되고 끊어지지 않도록 할 수 있습니다.

상자 크기 조정 속성에 대한 자세한 내용은 [CSS 상자 크기 조정 장](https://www.w3schools.com/css/css3_box-sizing.asp)에서 확인할 수 있다.

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

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_float_boxes_flex)

Flexbox의 유일한 문제점은 Internet Explorer 10 또는 이전 버전에서는 작동하지 않는다는 것이다. Flexbox Layout Module에 대한 자세한 내용은 [CSS Flexbox Chapter] (https://www.w3schools.com/css/css3_flexbox.asp)에서 확인할 수 있다.

------

## Navigation Menu

하이퍼 링크 목록과 함께 `float`을 사용하여 가로 메뉴를 만든다.

### 예제

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_float5)

------

## Web Layout Example

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
| [box-sizing](https://www.w3schools.com/cssref/css3_pr_box-sizing.asp) | 요소의 너비와 높이가 계산되는 방식을 정의한다. 패딩과 테두리를 포함해야하는지 여부 |
| [clear](https://www.w3schools.com/cssref/pr_class_clear.asp) | 지워진 요소 옆에 어떤 요소가 떠 다닐 수 있는지 지정          |
| [float](https://www.w3schools.com/cssref/pr_class_float.asp) | 요소가 떠 다니는 방법을 지정                                 |
| [overflow](https://www.w3schools.com/cssref/pr_pos_overflow.asp) | 내용이 요소 상자에 넘칠 경우 발생하는 상황을 지정한다        |
| [overflow-x](https://www.w3schools.com/cssref/css3_pr_overflow-x.asp) | 내용이 요소의 내용 영역에 넘칠 경우 내용의 왼쪽 / 오른쪽 가장자리로 수행 할 작업을 지정 |
| [overflow-y](https://www.w3schools.com/cssref/css3_pr_overflow-y.asp) | 내용이 요소의 내용 영역에 넘칠 경우 내용의 위쪽 / 아래쪽 가장자리로 수행 할 작업을 지정 |

[CSS inline-block](./CSS_inlineblock.md)