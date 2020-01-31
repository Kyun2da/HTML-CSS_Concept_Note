# CSS Padding

## CSS Padding

CSS padding 속성은 정의된 테두리 내에서 엘리먼트의 내용 주위에 공간을 생성하는데 사용된다.

CSS를 사용하면 패딩을 완전히 제어할 수 있다. 엘리먼트의 각 측면에는 패딩을 설정하는 속성이 있다.(위쪽, 오른쪽, 아래쪽, 왼쪽)

## Padding - Individual Sides

CSS는 각각의 엘리먼트의 면에 패딩을 사용할 수 있는 속성을 가지고 있다.

- `padding-top`
- `padding-right`
- `padding-bottom`
- `padding-left`

모든 패딩은 다음과 같은 값이 허용된다.

- *length* - 길이 px, pt, cm, etc
- *%* - 엘리먼트를 포함하는 넓이의 몇퍼센트
- inherit - 부모 엘리먼트로 부터 상속을 받을 수 있다.

**Note:** 음수는 허용되지 않는다.

### 예제

`<div>`엘리먼트의 네 면을 통해 다른 패딩을 쓸 수 있다.

```css
div {
 padding-top: 50px;
 padding-right: 30px;
 padding-bottom: 50px;
 padding-left: 80px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_padding_sides)

------

## Padding - Shorthand Property

코드를 짧게하기 위해서 `padding`을 사용해 하나의 속성으로 사용할 수 있다.

- `padding-top`
- `padding-right`
- `padding-bottom`
- `padding-left`

아래와 같이 작동한다.

만약 `padding` 속성이 네가지 값을 가지고 있다면

- padding: 25px 50px 75px 100px;
  - top padding is 25px
  - right padding is 50px
  - bottom padding is 75px
  - left padding is 100px

### 예제

네가지 값을 패딩의 짧은 코딩으로 사용하는 법

```css
div {
 padding: 25px 50px 75px 100px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_padding_shorthand_4val)

만약 `padding` 속성이 세가지 값을 가지고 있다면

- padding: 25px 50px 75px;
  - top padding is 25px
  - right and left paddings are 50px
  - bottom padding is 75px

### 예제

세가지 값을 패딩의 짧은 코딩으로 사용하는 법

```css
div {
 padding: 25px 50px 75px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_padding_shorthand_3val)

만약 `padding` 속성이 두가지 값을 가지고 있다면

- padding: 25px 50px;
  - top and bottom paddings are 25px
  - right and left paddings are 50px

### 예제

두가지 값을 패딩의 짧은 코딩으로 사용하는 법

```css
div {
 padding: 25px 50px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_padding_shorthand_2val)

만약 `padding` 속성이 한가지 값을 가지고 있다면

- padding: 25px;
  - all four paddings are 25px

### 예제

한가지 값을 패딩의 짧은 코딩으로 사용하는 법

div {
 padding: 25px;
}

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_padding_shorthand_1val)

------

## Padding and Element Width

CSS 넓이 속성은 엘리먼트 내용 영역의 너비를 지정한다. 내용 영역은 엘리먼트의 안쪽 여백, 테두리 및 여백 내부 부분이다.

따라서 요소에 지정된 너비가 있으면 해당 엘리먼트에 추가 된 패딩이 엘리먼트의 총 너비에 추가됩니다. 이것은 종종 바람직하지 않은 결과이다.

### 예제

여기에 `<div>`엘리먼트는 300px의 넓이로 주어진다. 그러나 실제 `<div>`엘리먼트는 350px이 될것이다. 왜냐하면 왼쪽 패딩 25 + 오른쪽패딩 25를 더해야하므로

```css
div {
 width: 300px;
 padding: 25px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_padding_width)

넓이 300px을 유지하기 위해서는 패딩의 양은 상관없고 너는 `box-sizing`이라는 속성을 사용할 수 있다 이것은 그것의 넓이를 유지시켜주며 만약 너가 패딩을 늘리면 그 내용 공간을 줄이게 된다.

### 예제

```css
div {
 width: 300px;
 padding: 25px;
 box-sizing: border-box;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_padding_width2)



------

## 모든 CSS padding 속성

| 속성                                                         | 설명                                                         |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [padding](https://www.w3schools.com/cssref/pr_padding.asp)   | A shorthand property for setting all the padding properties in one declaration |
| [padding-bottom](https://www.w3schools.com/cssref/pr_padding-bottom.asp) | 아래쪽 padding의 속성을 정의함                               |
| [padding-left](https://www.w3schools.com/cssref/pr_padding-left.asp) | 왼쪽 padding의 속성을 정의함                                 |
| [padding-right](https://www.w3schools.com/cssref/pr_padding-right.asp) | 오른쪽 padding의 속성을 정의함                               |
| [padding-top](https://www.w3schools.com/cssref/pr_padding-top.asp) | 위쪽 padding의 속성을 정의함                                 |

[CSS Height and Width](./CSS_handw.md)