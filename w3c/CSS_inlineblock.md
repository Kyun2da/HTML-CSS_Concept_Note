# CSS Layout - display: inline-block

## The display: inline-block Value

`display : inline`과 비교할 때 가장 큰 차이점은`display : inline-block`은 요소의 너비와 높이를 설정할 수 있다는 것이다.

또한 'display : inline-block'을 사용하면 위쪽 및 아래쪽 여백 / 패딩이 존중되지만`display : inline '은 그렇지 않다.

`display : block`과 비교할 때 주요 차이점은`display : inline-block`은 요소 다음에 줄 바꿈을 추가하지 않으므로 요소가 다른 요소 옆에있을 수 있다는 것입니다.

다음 예제는`display : inline`,`display : inline-block` 및`display : block`의 다른 동작을 보여준다.

### 예제

```css
span.a {
 display: inline; /* the default for span */
 width: 100px;
 height: 100px;
 padding: 5px;
 border: 1px solid blue;
 background-color: yellow;
}

span.b {
 display: inline-block;
 width: 100px;
 height: 100px;
 padding: 5px;
 border: 1px solid blue;
 background-color: yellow;
}

span.c {
 display: block;
 width: 100px;
 height: 100px;
 padding: 5px;
 border: 1px solid blue;
 background-color: yellow;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_inline-block_span1)

------

## Using inline-block to Create Navigation Links

`display : inline-block`의 일반적인 용도 중 하나는 목록 항목을 세로가 아닌 가로로 표시하는 것이다. 다음 예제는 가로 탐색 링크를 작성한다.

### 예제

```css
.nav {
 background-color: yellow;
 list-style-type: none;
 text-align: center; 
 padding: 0;
 margin: 0;
}

.nav li {
 display: inline-block;
 font-size: 20px;
 padding: 20px;
}
```

[CSS Align](./CSS_align.md)