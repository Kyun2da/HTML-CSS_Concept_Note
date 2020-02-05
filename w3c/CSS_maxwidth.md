# CSS Layout - width and max-width

## width, max-width, margin :auto 를 사용하기

전 챕터에서 언급한 것 처럼 블록 수준 엘리먼트는 항상 가능한 최대의 넓이를 가진다.

블록수준의 엘리먼트의 넓이를 세팅하는 것은 그것이 그것의 컨테이너의 테두리밖으로 뻗는것을 못하게 해준다. 그때 너는 마진을 auto로 셋팅할 수 있고 그것의 컨테이너안에 엘리먼트를 수평적으로 중앙에 놓을 수 있다. 이 엘리먼트는 특수한 넓이를 가지고 공간을 일정하게 두개의마진으로 놓고 중앙에 정렬할 것이다.



**Note:** 위의 `<div>` 문제는 브라우저 창이 요소 너비보다 작을 때 발생한다. 그런 다음 브라우저는 페이지에 가로 스크롤 막대를 추가합니다.

이 상황에서 최대 너비를 대신 사용하면 브라우저의 작은 창 처리가 향상된다. 소형 장치에서 사이트를 사용할 수있게 할 때 중요하다.

**Tip:** 두 div의 차이점을 보려면 브라우저 창 크기를 500px 미만으로 조정해라!

여기에 두개의 div의 예제가 있다.

### 예제

```css
div.ex1 {
 width: 500px;
 margin: auto;
 border: 3px solid #73AD21;
}

div.ex2 {
 max-width: 500px;
 margin: auto;
 border: 3px solid #73AD21;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_max-width)

[CSS Position](./CSS_position.md)