

## The CSS Box Model

모든 HTML 엘리먼트는 박스로 고려될 수 있다. CSS에서 box model이라는 용어는 디자인과 레이아웃에 관해 이야기할 때 사용된다.

CSS box모델은 모든 HTML 엘리먼트에 감싸진 박스이다. 이것은 마진, 테두리, 패딩, 그리고 실제 내용으로 구성 된다.

다른 부분을 설명한다.

- **Content** - 텍스트와 이미지가 나타나는 곳이며 박스의 내용부분이다.
- **Padding** - 내용주위 의구역이며 패딩은 투명하다.
- **Border** - 내용과 패딩을 감싸는 테두리를 말한다.
- **Margin** - 테두리 밖의 내용을 말하며 투명하다.

박스 모델은 우리에게 테두리와 주변의 엘리먼트를 추가하는 것을 허락하고 엘리먼트의 사이의 공간 또한 정의할 수 있다.

### 예제

박스모델의 설명

```css
div {
 width: 300px;
 border: 15px solid green;
 padding: 50px;
 margin: 20px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_boxmodel)



## Width and Height of an Element

모든 브라우저에서 요소의 너비와 높이를 올바르게 설정하려면 상자 모델의 작동 방식을 알아야한다.

**Important: **CSS를 사용하여 요소의 너비 및 높이 속성을 설정하면 내용 영역의 너비와 높이 만 설정하면된다. 요소의 전체 크기를 계산하려면 안쪽 여백, 테두리 및 여백도 추가해야한다.

### 예제

이 `<div>`엘리먼트는 총 350픽셀이다.

```css
div {
 width: 320px;
 padding: 10px;
 border: 5px solid gray;
 margin: 0;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_boxmodel_width)

아래는 계산하는 법이다.

320px (width)
\+ 20px (left + right padding)
\+ 10px (left + right border)
\+ 0px (left + right margin)
**= 350px**

요소의 총 너비는 다음과 같이 계산해야한다. 

총 요소 너비 = 너비 + 왼쪽 여백 + 오른쪽 여백 + 왼쪽 테두리 + 오른쪽 테두리 + 왼쪽 여백 + 오른쪽 여백 

요소의 총 높이는 다음과 같이 계산해야한다. 

총 요소 높이 = 높이 + 위쪽 패딩 + 아래쪽 패딩 + 위쪽 테두리 + 아래쪽 테두리 + 위쪽 여백 + 아래쪽 여백

[CSS Outline](./CSS_outline.md)