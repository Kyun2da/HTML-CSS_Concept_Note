# CSS Syntax

## CSS Syntax

CSS 규약은 선택자와 선언 블록으로 구성되어있다.

![CSS 이미지](https://www.w3schools.com/css/selector.gif)

선택자는 너가 스타일링 하고싶은 HTML 을 가리킨다.

선언 블록은 한개나 더많은 세미콜론에 의해 분리된 선언을 포함한다.

각각의 선언은 CSS속성이름과 값을 포함하고 콜론에의해 분리된다.

CSS 선언은 항상 세미콜론으로 끝나고 선언 블록은 중괄호로 둘러싸인다.



### 예제

이 예제는 `<p>`태그를 중앙정렬하고 빨간색으로 바꾸는 코드이다.

```css
p {
 color: red;
 text-align: center;
}
```



## CSS 코멘트

코멘트는 설명 블록으로 둘러싸이고 이것은 너가 소스코드에 대해 코멘트를 남기고 싶을 때 사용한다.

코멘트는 브라우저에서는 거부된다.

### 예제

CSS에서 코멘트는 /*로 시작해서 */로 끝난다. 코멘트는 여러줄이 될 수 있다.

```css
p {
 color: red;
 /* This is a single-line comment */
 text-align: center;
}

/* This is
a multi-line
comment */
```

[CSS Selectors](./CSS_selector.md)

