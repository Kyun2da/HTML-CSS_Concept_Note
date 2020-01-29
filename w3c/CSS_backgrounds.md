# CSS Backgrounds

CSS 배경속성은 엘리먼트에 배경효과를 정의하는데에 사용된다.

CSS 배경속성

- background-color
- background-image
- background-repeat
- background-attachment
- background-position

------

## CSS background-color

 `background-color` 속성은 배경색을 정의할 때 쓰인다.

### 예제

배경색은 다음과 같이 정할 수 있다.

```css
body {
 background-color: lightblue;
}
```



CSS에서 색은 다음과 같이 정의될 수 있다.

- a valid color name - like "red"
- a HEX value - like "#ff0000"
- an RGB value - like "rgb(255,0,0)"

### 예제

여기에 h1, p, div 의 색상을 정의 해놓았다. 

```css
h1 {
 background-color: green;
}

div {
 background-color: lightblue;
}

p {
 background-color: yellow;
}
```



## CSS background-image

 `background-image` 속성은 엘리먼트의 배경으로써 사용하기위해 이미지를 가져다올 때 사용한다.

기본적으로 이미지는 그것이 전체 엘리먼트를 커버할때까지 반복된다.

### 예제

배경이미지는 다음과 같이 적용될 수 있다.

```css
body {
 background-image: url("paper.gif");
}
```



### 예제

아래 예는 텍스트와 배경이미지의 나쁜 조합을 보여준다 이 텍스트는 읽기 어렵다

```scss
body {
 background-image: url("bgdesert.jpg");
}
```



**Note:** 배경이미지를 사용할때 텍스트에 혼잡을 주는 이미지는 사용해선 안된다.

------

## CSS background-repeat

기본적으로 `background-image` 속성은 이미지를 수평과 수직적으로 반복한다.

몇몇 이미지들은 수평또는 수직적으로만 반복될 수 있고 이것은 이상해보일 수있다 아래예제처럼

### 예제

```css
body {
 background-image: url("gradient_bg.png");
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_background-image_gradient1)

만약 이미지가 단지 수직적으로 반복된다면 아래의 속성을 써서 백그라운드를 더 보기 좋게 바꿀 수 있다.

### 예제

```css
body {
 background-image: url("gradient_bg.png");
 background-repeat: repeat-x;
}
```



**Tip:** 이미지를 수평적으로 반복하기 위해서는 `background-repeat: repeat-y;`로 바꾸면 된다.

------

## CSS background-repeat: no-repeat

배경 이미지를 한번만 보여주는것은 background-repeat속성으로 지정할 수 있다.

### 예제

배경 이미지를 한번만 보여주는 예제이다.

```css
body {
 background-image: url("img_tree.png");
 background-repeat: no-repeat;
}
```

위 예제에서 배경 이미지는 텍스트와 같은 위치에 위치한다. 우리는 이러한 이미지의 포지션을 바꾸고 싶다. 왜냐하면 그것이 텍스트를 방해하기 때문이다.

------

## CSS background-position

 `background-position` 속성은 배경 이미지의 위치를 구체화시키는데에 사용된다.

### 예제

배경이미지를 오른쪽 위로 몰아넣는 예제이다.

```css
body {
 background-image: url("img_tree.png");
 background-repeat: no-repeat;
 background-position: right top;
}
```



------

## CSS background-attachment

 `background-attachment` 속성은 배경 이미지가 고정되거나 스크롤될 수있을지를 결정하는 속성이다.

### 예제

아래 예제는 배경을 스크롤해도 고정하는 것이다.

```css
body {
 background-image: url("img_tree.png");
 background-repeat: no-repeat;
 background-position: right top;
 background-attachment: fixed;
}
```



### 예제

Specify that the background image should scroll with the rest of the page:

```css
body {
 background-image: url("img_tree.png");
 background-repeat: no-repeat;
 background-position: right top;
 background-attachment: scroll;
}
```



------

## CSS background - Shorthand 속성

코드를 짧게 쓰기 위해서 위의 속성들을 background 속성 하나에 몰아쓰는 것이 가능하다. 이것을 shorthand 속성이라고 부른다.

이 shorthand 속성은 배경을위한 속성이며 background라고 쓴다.

### 예제

shorthand 속성을 사용하여 아래처럼 하나의 선언으로 끝낸 것이다.

```css
body {
 background: #ffffff url("img_tree.png") no-repeat right top;
}
```



shorthand 속성을 사용할때는 다음의 순서를 따른다.

- `background-color`
- `background-image`
- `background-repeat`
- `background-attachment`
- `background-position`

이것은 하나의 속성이 안쓰져있다고 해도 다른속성이 순서를 잘 지키고 있는한은 상관없다.

------

## 모든 CSS 배경 속성

| 속성                                                         | 설명                                                  |
| :----------------------------------------------------------- | :---------------------------------------------------- |
| [background](https://www.w3schools.com/cssref/css3_pr_background.asp) | 모든 background 속성을 하나의 속성으로 바꾸는 것이다. |
| [background-attachment](https://www.w3schools.com/cssref/pr_background-attachment.asp) | 배경 이미지를 고정 혹은 스크롤할때 결정하는 것이다.   |
| [background-clip](https://www.w3schools.com/cssref/css3_pr_background-clip.asp) | 배경의 페인팅할 구역을 정해놓는 것이다.               |
| [background-color](https://www.w3schools.com/cssref/pr_background-color.asp) | 엘리먼트의 배경색을 지정하는 것이다.                  |
| [background-image](https://www.w3schools.com/cssref/pr_background-image.asp) | 엘리먼트의 배경이미지를 지정하는 것이다.              |
| [background-origin](https://www.w3schools.com/cssref/css3_pr_background-origin.asp) | 배경이미지의 위치를 어디에 둘지 지정하는 것이다.      |
| [background-position](https://www.w3schools.com/cssref/pr_background-position.asp) | 배경 이미지의 시작 위치를 지정하는 것이다.            |
| [background-repeat](https://www.w3schools.com/cssref/pr_background-repeat.asp) | 배경 이미지가 어떻게 반복될지 지정하는 것이다.        |
| [background-size](https://www.w3schools.com/cssref/css3_pr_background-size.asp) | 배경이미지의 사이즈를 결정하는 것이다.                |

[CSS Borders](./CSS_borders.md)

