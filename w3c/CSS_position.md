# CSS Layout - The position Property

## The position Property

`<position>`속성은 엘리먼트에 위치를 정하는 타입이다.

- `static`
- `relative`
- `fixed`
- `absolute`
- `sticky`

엘리먼트들은 top,bottom,left,right 속성을 사용하여 위치된다. 그러나 이러한 속성은 position속성을 처음 세팅하지않으면 동작하지 않는다. 그것들은 position 값에 따라 다르게 동작한다.

------

## position: static;

HTML엘리먼트는 기본적으로  static값의 위치를 갖는다.

static 엘리먼트는 top, bottom, left, right속성에 의해 영향을 미치지 않는다.

### 예제

```css
div.static {
 position: static;
 border: 3px solid #73AD21;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_position_static)

------

## position: relative;

`position : relative`를 가진 엘리먼트는 그것의 일반적인 위치에 상대적인 위치로 위치해있다.

상대적으로 배치 된 요소의 위쪽, 오른쪽, 아래쪽 및 왼쪽 속성을 설정하면 일반 위치에서 멀어 지도록 조정된다. 다른 내용은 요소가 남긴 간격에 맞게 조정되지 않는다.

### 예제

```css
div.relative {
 position: relative;
 left: 30px;
 border: 3px solid #73AD21;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_position_relative)

------

## position: fixed;

`position : fixed;`이있는 요소는 뷰포트를 기준으로 배치되므로 페이지가 스크롤 되더라도 항상 같은 위치에 유지된다. top, right, bottom 및 left 속성은 요소를 배치하는 데 사용된다.

고정 요소는 일반적으로 위치했던 페이지에 공백을 남기지 않는다.

페이지 오른쪽 하단에 고정 요소가 있다. 사용되는 CSS는 다음과 같다.

### 예제

```css
div.fixed {
 position: fixed;
 bottom: 0;
 right: 0;
 width: 300px;
 border: 3px solid #73AD21;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_position_fixed)

------

## position: absolute;

`position : absolute;`가있는 요소는 고정 된 것처럼 뷰포트를 기준으로 배치 된 대신 가장 가까운 위치를 둔 조상에 대해 배치된다.

그러나 절대 위치 요소에 위치 조상이 없으면 문서 본문을 사용하고 페이지 스크롤과 함께 이동한다.

**Note:** "위치"요소는 위치가 '정적'이외의 요소이다.

다음은 간단한 예다.

이 <div> 요소는 position : relative;

이 <div> 요소는 position : absolute;

사용되는 CSS는 다음과 같다.

### 예제

```css
div.relative {
 position: relative;
 width: 400px;
 height: 200px;
 border: 3px solid #73AD21;
}

div.absolute {
 position: absolute;
 top: 80px;
 right: 0;
 width: 200px;
 height: 100px;
 border: 3px solid #73AD21;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_position_absolute)

------

## position: sticky;

`position : sticky;`가있는 요소는 사용자의 스크롤 위치를 기준으로 배치된다.

스티커 요소는 스크롤 위치에 따라 '상대적'과 '고정적'사이를 토글한다. 주어진 오프셋 위치가 뷰포트에서 충족 될 때까지 상대적으로 배치 된 다음 위치에 고정된다 (예 : 위치 : 고정).

**Note: **Internet Explorer, Edge 15 및 이전 버전은 고정 위치를 지원하지 않는다. Safari에는 -webkit- 접두사가 필요하다 (아래 예 참조). 또한 고정 위치 지정이 작동하려면`top`,`right`,`bottom` 또는`left` 중 하나 이상을 지정해야한다.

이 예에서, 고정 위치는 스크롤 위치에 도달 할 때 페이지 상단 (`top : 0`)에 고정된다.

### 예제

```css
div.sticky {
 position: -webkit-sticky; /* Safari */
 position: sticky;
 top: 0;
 background-color: green;
 border: 2px solid #4CAF50;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_position_sticky)

------

## Overlapping Elements

엘리먼트가 위치될 때 그것들은 다른 엘리먼트를 오버랩할 수 있다.

z-index속성은 엘리먼트의 순서로 쌓인다.

엘리먼트는 + 또는 - 값을 가질 수 있다.

### 예제

```css
img {
 position: absolute;
 left: 0px;
 top: 0px;
 z-index: -1;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_zindex)

스택 순서가 큰 요소는 항상 스택 순서가 낮은 요소 앞에 있다.

**Note:** 'z- 인덱스'를 지정하지 않고 두 개의 위치 지정된 요소가 겹치면 HTML 코드에서 마지막에있는 요소가 맨 위에 표시된다.

------

## All CSS Positioning Properties

| 속성                                                         | 설명                                       |
| :----------------------------------------------------------- | :----------------------------------------- |
| [bottom](https://www.w3schools.com/cssref/pr_pos_bottom.asp) | 배치 된 상자의 아래쪽 여백 가장자리를 설정 |
| [clip](https://www.w3schools.com/cssref/pr_pos_clip.asp)     | 절대 위치 요소를 자른다                    |
| [left](https://www.w3schools.com/cssref/pr_pos_left.asp)     | 배치 된 상자의 왼쪽 여백 가장자리를 설정   |
| [position](https://www.w3schools.com/cssref/pr_class_position.asp) | 요소의 위치 지정 유형을 지정               |
| [right](https://www.w3schools.com/cssref/pr_pos_right.asp)   | 배치 된 상자의 오른쪽 여백 가장자리를 설정 |
| [top](https://www.w3schools.com/cssref/pr_pos_top.asp)       | 배치 된 상자의 상단 여백 가장자리를 설정   |
| [z-index](https://www.w3schools.com/cssref/pr_pos_z-index.asp) | 요소의 스택 순서를 설정                    |

[CSS Layout - Overflow](./CSS_overflow.md)