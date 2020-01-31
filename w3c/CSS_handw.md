# CSS Height and Width

## CSS Setting height and width

`height `  와 `width`속성은 엘리먼트의 높이와 넓이를 정의하는데 사용한다.

------

## CSS height/width Values

 `height` 와 `width` 속성은 아래와 같은 값을 허용한다.

- `auto` - 기본 값이다. 브라우저는 높이와 넓이를 계산한다.
- `length` - height/width를  px, cm etc의 단위로 정의한다
- `%` - 포함하는 블록의 %로 정의한다
- `initial` - height/width를 기본 값으로 세팅한다.
- `inherit` - 부모 값으로 상속한다

------

## CSS height/width Examples

높이는 200px이고 넓이는 50%이다

### 예제

`<div>`엘리먼트의 넓이와 높이를 세팅한다.

```css
div {
 height: 200px;
 width: 50%;
 background-color: powderblue;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_dim_height_width2)

이 엘리먼트는 500픽셀의넓이와 100픽셀의 높이를 가지고 있다.

### 예제

`<div>`엘리먼트의 높이와 넓이를 세팅한다.

```css
div {
 height: 100px;
 width: 500px;
 background-color: powderblue;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_dim_height_width)

**Note:** 높이와 넓이 속성은 padding, border margin을 포함하지 않는다. 그것들은 엘리먼트 안의 margin, border, padding안의 구역의 넓이와 높이를 설정하는 것이다.

## 최대 넓이를 설정하기

max-width 속성은 요소의 최대 너비를 설정하는 데 사용된다.

최대 너비는 px, cm 등의 길이 값 또는 포함하는 블록의 백분율 (%)로 지정하거나 none (이는 기본값이다. 최대 너비가 없음을 의미)으로 설정할 수 있다.

위의 <div> 문제는 브라우저 창이 요소 너비 (500px)보다 작을 때 발생한다. 그런 다음 브라우저는 페이지에 가로 스크롤 막대를 추가한다.

이 상황에서 최대 너비를 대신 사용하면 브라우저의 작은 창 처리가 향상된다.

팁 : 두 div의 차이점을 보려면 브라우저 창을 500px 미만으로 드래그해라!

### 예제

이 `<div>`엘리먼트는 100픽셀의 높이와 500픽셀의 최대 넓이를 가진다.

```css
div {
 max-width: 500px;
 height: 100px;
 background-color: powderblue;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_dim_max_width)



## 모든 CSS 차원 속성

| 속성                                                         | 설명                            |
| :----------------------------------------------------------- | :------------------------------ |
| [height](https://www.w3schools.com/cssref/pr_dim_height.asp) | 엘리먼트의 높이를 설정한다      |
| [max-height](https://www.w3schools.com/cssref/pr_dim_max-height.asp) | 엘리먼트의 최대 높이를 설정한다 |
| [max-width](https://www.w3schools.com/cssref/pr_dim_max-width.asp) | 엘리먼트의 최대 넓이를 설정한다 |
| [min-height](https://www.w3schools.com/cssref/pr_dim_min-height.asp) | 엘리먼트의 최소 길이를 설정한다 |
| [min-width](https://www.w3schools.com/cssref/pr_dim_min-width.asp) | 엘리먼트의 최소 넓이를 설정한다 |
| [width](https://www.w3schools.com/cssref/pr_dim_width.asp)   | 엘리먼트의 넓이를 설정한다      |

[CSS Box Model](./CSS_box.md)

