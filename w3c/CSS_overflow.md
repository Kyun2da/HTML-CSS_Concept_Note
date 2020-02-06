# CSS Layout - Overflow

CSS overflow 속성은 너무 커서 영역에 맞지 않는 내용의 내용을 제어합니다.
[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_overflow_intro)

------

## CSS Overflow

'overflow'속성은 요소의 내용이 너무 커서 지정된 영역에 맞지 않을 때 내용을자를 것인지 스크롤 막대를 추가 할 것인지를 지정한다.

 `overflow` 속성은 다음과 같은 값들을 갖고있다.

- `visible` - 기본값이다. 오버 플로우가 잘리지 않는다. 내용은 요소 상자 외부에서 렌더링된다.

- `hidden` - 오버플로가 잘리고 나머지 내용은 보이지 않는다.

- `scroll` - 오버플로가 잘리고 스크롤 막대가 추가되어 나머지 내용을 볼 수 있다.

- `auto` - `scroll`과 비슷하지만 필요할 때만 스크롤바를 추가한다.

  **Note:**	`overflow`속성은 지정된 높이를 가진 블록 요소에 대해서만 작동한다.

------

## overflow: visible

기본적으로 오버플로는 '보이는 것'이다. 즉, 잘리지 않으며 요소 상자 외부에서 렌더링된다.

레이아웃을보다 잘 제어하려면 overflow 속성을 사용할 수 있다. overflow 속성은 내용이 요소 상자에 넘칠 경우 발생하는 상황을 지정한다.

### 예제

```css
div {
 width: 200px;
 height: 50px;
 background-color: #eee;
 overflow: visible;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_overflow_visible)

## overflow: hidden

'hidden'값을 사용하면 오버플로가 잘리고 나머지 내용은 숨겨진다.

레이아웃을보다 잘 제어하려면 overflow 속성을 사용할 수 있다. overflow 속성은 내용이 요소 상자에 넘칠 경우 발생하는 상황을 지정한다.

### 예제

```css
div {
 overflow: hidden;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_overflow_hidden)

------

## overflow: scroll

값을 'scroll'로 설정하면 오버플로가 잘리고 상자 안에 스크롤 막대가 추가된다. 이렇게하면 스크롤 막대가 가로 및 세로로 추가된다 (필요하지 않더라도).

레이아웃을보다 잘 제어하려면 overflow 속성을 사용할 수 있다. overflow 속성은 내용이 요소 상자에 넘칠 경우 발생하는 상황을 지정한다.

### 예제

```css
div {
 overflow: scroll;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_overflow_scroll)

------

## overflow: auto

`auto` 값은`scroll`과 비슷하지만 필요할 때만 스크롤바를 추가한다 :

레이아웃을보다 잘 제어하려면 overflow 속성을 사용할 수 있다. overflow 속성은 내용이 요소 상자에 넘칠 경우 발생하는 상황을 지정한다.

### 예제

```css
div {
 overflow: auto;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_overflow_auto)

------

## overflow-x and overflow-y

'overflow-x'및 'overflow-y'속성은 컨텐츠의 오버플로를 가로 또는 세로로만 변경할지 아니면 둘 다로 변경 할지를 지정한다.

'overflow-x'는 컨텐츠의 왼쪽 / 오른쪽 가장자리로 수행 할 작업을 지정한다.
'overflow-y'는 컨텐츠의 상단 / 하단 가장자리와 관련하여 수행 할 작업을 지정한다.

레이아웃을보다 잘 제어하려면 overflow 속성을 사용할 수 있다. overflow 속성은 내용이 요소 상자에 넘칠 경우 발생하는 상황을 지정한다.

### 예제

```css
div {
 overflow-x: hidden; /* Hide horizontal scrollbar */
 overflow-y: scroll; /* Add vertical scrollbar */
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_overflow_xy)

------

## All CSS Overflow Properties

| 속성                                                         | 설명                                                         |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [overflow](https://www.w3schools.com/cssref/pr_pos_overflow.asp) | 내용이 요소 상자에 넘칠 경우 발생하는 상황을 지정            |
| [overflow-x](https://www.w3schools.com/cssref/css3_pr_overflow-x.asp) | 내용이 요소의 내용 영역에 넘칠 경우 내용의 왼쪽 / 오른쪽 가장자리로 수행 할 작업을 지정 |
| [overflow-y](https://www.w3schools.com/cssref/css3_pr_overflow-y.asp) | 내용이 요소의 내용 영역에 넘칠 경우 내용의 위쪽 / 아래쪽 가장자리로 수행 할 작업을 지정 |

[CSS float](./CSS_float.md)

