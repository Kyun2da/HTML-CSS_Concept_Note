# CSS Margins

## CSS Margins

CSS `margin` 속성은 엘리먼트 주변의 공간을 만들기위해 사용된다. 테두리의 바깥 공간을 말한다.

CSS에서 너는 마진을 컨트롤할 수 있다. 각각의 왼쪽 오른쪽 위 아래의 마진을 지정하는 속성이 있다.

------

## Margin - Individual Sides

CSS는 각각의 엘리먼트에 대한 마진을 설정하는데에 특화되어 있다.

- `margin-top`
- `margin-right`
- `margin-bottom`
- `margin-left`

모든 마진 속성들은 다음과 같은 값을 가지고 있다.

- auto - 브라우저는 마진을 계산한다.
- *length* - 마진을 px, pt, cm, 기타 등등으로 특화시킨다.
- *%* - 엘리먼트를 포함한 넓이를 %로 정의할 수 있다.
- inherit - 부모 엘리먼트로부터 마진이 상속 된다.

**Tip:** 음수 또한 허용이 된다.

### 예제

`<p>`앨리먼트의 네쪽 면을 다른 마진으로 설정한다.

p {
 margin-top: 100px;
 margin-bottom: 100px;
 margin-right: 150px;
 margin-left: 80px;
}

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_margin_sides)

## Margin - Shorthand Property

코드를 짧게 쓰기위해 하나의 속성으로 모든 마진 속성을 특화 시키는 것이 가능하다.

`margin` 속성은 각각의 마진속성의 축약된 속성이다.

- `margin-top`
- `margin-right`
- `margin-bottom`
- `margin-left`

아래에 어떻게 동작하는지 나온다.

만약 `margin` 속성이 네개의 값을 가지고 있다면

- margin: 25px 50px 75px 100px;
  - top 마진은 25px
  - right 마진은 50px
  - bottom 마진은 75px
  - left 마진은 100px

### 예제

4개의 값으로 마진속성을 사용하면

```css
p {
 margin: 25px 50px 75px 100px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_margin_shorthand_4val)

만약 `margin` 속성이 3가지 값을 갖는다면

- margin: 25px 50px 75px;
  - top 마진은 25px
  - 오른쪽과 왼쪽 마진은 50px
  - 아래 마진은 75px

### 예제

짧게 세가지의 값을 사용한다면 아래와 같이 쓸 수 있다.

```css
p {
 margin: 25px 50px 75px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_margin_shorthand_3val)

만약 `margin` 속성이 두가지 값을 갖는 다면

- margin: 25px 50px;
  - top 과 bottom 마진은 25px
  - right 과 left 마진은 50px

### 예제

마진을 짧은 두가지의 값으로 사용해라

```css
p {
 margin: 25px 50px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_margin_shorthand_2val)

만약 `margin` 속성이 하나의 값을 갖는다면

- margin: 25px;
  - 모든 4개의 마진은 25px

### 예제

하나의 값으로 짧게 마진을 쓴다면

```css
p {
 margin: 25px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_margin_shorthand_1val)

------

## 자동 값

너는 마진의 속성을 `auto`로 저장할수 있다. 이는 컨테이너 내에서 앨리먼트를 가운데에 맞출 수 있도록 해준다

그러면 앨리먼트가 지정된 너비를 차지하고 남은 공간이 왼쪽과 오른쪽 여백 사이를 균등하게 분할한다.

### 예제

마진을 auto값으로 사용하기:

div {
 width: 300px;
 margin: auto;
 border: 1px solid red;
}

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_margin_auto)

------

## 상속값

이 예제는 왼쪽 마진을 부모 앨리먼트 `<div>`에 줘서 자손 앨리먼트인 p 클래스를 왼쪽 마진이 생기도록 하는 예제이다.

### 예제

상속값을 다음과 같이 쓸 수 있다.

```css
div {
 border: 1px solid red;
 margin-left: 100px;
}

p.ex1 {
 margin-left: inherit;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_margin-left_inherit)

------

## Margin Collapse

앨리먼트의 위쪽 및 아래쪽 여백이 두 여백 중 가장 큰 단일 여백으로 축소되는 경우가 있다.

왼쪽 및 오른쪽 여백에서는 발생하지 않고 위와 아래쪽 여백에만 발생하게된다.

### 예제

margin collapse를 설명하는 예이다.

```css
h1 {
 margin: 0 0 50px 0;
}

h2 {
 margin: 20px 0 0 0;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_margin_collapse)

위의 예에서 `<h1>`요소의 아래쪽 여백은 50px 이고 `<h2>`요소의 위쪽 여백은 20px로 설정되어 있다. 생각대로라면 50+20인 70px을 의미해야할 것 같지만 마진 축소로 인해 실제 마진은 50px을 의미한다.

------

## All CSS Margin Properties

| 속성                                                         | 설명                                          |
| :----------------------------------------------------------- | :-------------------------------------------- |
| [margin](https://www.w3schools.com/cssref/pr_margin.asp)     | 하나의 선언으로 마진 속성들을 셋팅할 수 있다. |
| [margin-bottom](https://www.w3schools.com/cssref/pr_margin-bottom.asp) | bottom 앨리먼트의 마진을 정의한다.            |
| [margin-left](https://www.w3schools.com/cssref/pr_margin-left.asp) | left 앨리먼트의 마진을 정의한다.              |
| [margin-right](https://www.w3schools.com/cssref/pr_margin-right.asp) | right 앨리먼트의 마진을 정의한다.             |
| [margin-top](https://www.w3schools.com/cssref/pr_margin-top.asp) | top 앨리먼트의 마진을 정의한다.               |

[CSS Padding](./CSS_padding.md)

