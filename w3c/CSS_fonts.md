# CSS Fonts

[❮ Previous](https://www.w3schools.com/css/css_text.asp)[Next ❯](https://www.w3schools.com/css/css_icons.asp)

------

CSS 폰트속성은 텍스트의 스타일, 사이즈, 굵기, 폰트유형을 정의한다.

------

## Difference Between Serif and Sans-serif Fonts

![Serif vs. Sans-serif](https://www.w3schools.com/css/serif.gif)

------

## CSS Font Families

CSS에서 font-family의 두가지 유형이 있다.

- **generic family** - 보기에 비슷해보이는 font familiy의 그룹이다.
- **font family** - 특정한 font family다. (Times New Roman 혹은 Arial과 같은..)

| Generic family | Font family                | Description                                                  |
| :------------- | :------------------------- | :----------------------------------------------------------- |
| Serif          | Times New Roman Georgia    | 일부 문자의 세리프 글꼴 끝에 작은 줄이 있습니다              |
| Sans-serif     | Arial Verdana              | "산"은없는 것을 의미합니다.이 글꼴은 문자 끝에 줄이 없습니다. |
| Monospace      | Courier New Lucida Console | 모든 모노 스페이스 문자의 너비는 동일합니다                  |

**Note:** 컴퓨터 화면에서 sans-serif 글꼴은 serif 글꼴보다 읽기 쉬운 것으로 간주된다.

------

## Font Family

텍스트의 폰트 패밀리는 `font-family`속성으로 세팅된다.

`font-family` 속성에는 "대체"시스템으로 여러 글꼴 이름이 있어야한다. 브라우저가 첫 번째 글꼴을 지원하지 않으면 다음 글꼴 등을 시도한다.

다른 글꼴을 사용할 수없는 경우 브라우저가 일반 패밀리에서 유사한 글꼴을 선택할 수 있도록 원하는 글꼴로 시작하고 일반 패밀리로 끝난다.

**Note**: 글꼴 모음 이름이 두 단어 이상인 경우 "Times New Roman"과 같이 따옴표로 묶어야한다.

쉼표로 구분 된 목록에 둘 이상의 글꼴 패밀리가 지정되어있다.

### 예제

```css
p {
 font-family: "Times New Roman", Times, serif;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_font-family)

일반적인 유저 폰트의 조합을 보려면 이곳을 참조해라 [Web Safe Font Combinations](https://www.w3schools.com/cssref/css_websafe_fonts.asp).

------

## Font Style

 `font-style` 속성은 특수한 이탤릭체가 사용되곤 한다.

이 속성은 세가지의 값을 갖고 있다.

- normal - 텍스트가 일반적으로 보여진다.
- italic - 텍스트가 이탤릭체로 보여진다.
- oblique - 텍스트가 기울어져있다. (이탤릭체와 비슷하지만 덜 지원된다.)

### 예제

```css
p.normal {
 font-style: normal;
}

p.italic {
 font-style: italic;
}

p.oblique {
 font-style: oblique;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_font-style)

------

## Font Size

 `font-size` 속성은 텍스트의 사이즈를 지정한다.

웹 디자인에서 텍스트 크기를 관리 할 수 있어야 한다. 그러나 단락을 제목처럼 보이거나 제목을 단락처럼 보이도록 글꼴 크기 조정을 사용해서는 안된다.

제목에는 `h1~ h6` 단락에는 `p`와 같은 올바른 HTML 태그를 항상 사용해라

폰트크기는 절대적이거나 상대적인 크기를 갖는다.

절대적 크기:

- 텍스트를 지정된 크기로 설정한다.
- 사용자가 모든 브라우저에서 텍스트 크기를 변경할 수 없다.
- 절대 크기는 출력의 실제 크기를 알 때 유용하다.

상대적 크기:

- 주변 요소를 기준으로 크기를 설정한다
- 사용자가 브라우저에서 텍스트 크기를 변경할 수 있다.

**Note:** 글꼴 크기르 지정하지 않으면 단락과 같은 일반 텍스트의 기본 크기는 16px이다.

------

## Set Font Size With Pixels

텍스트 크기를 픽셀로 설정하면 텍스트 크기를 완전히 제어할 수 있다.

### 예제

```css
h1 {
 font-size: 40px;
}

h2 {
 font-size: 30px;
}

p {
 font-size: 14px;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_font-size_px)

**Tip:** 픽셀을 사용하는 경우에도 확대 도구를 사용하여 전체 페이지의 크기를 조정할 수 있다.

------

## Set Font Size With Em

사용자가 브라우저 메뉴에서 텍스트의 크기를 조정할 수 있도록 많은 개발자가 픽셀 대신 em을 사용한다.

em 크기 단위는 w3c에서 권장한다.

1em은 현재 글꼴 크기와 같다. 브라우저의 기본 텍스트 크기는 16px이다. 따라서 1em의 기본 크기는 16px이다.

다음 공식을 사용하여 픽셀에서 em 까지 크기를 계산할 수 있다.

pixels / 16 = em

### 예제

```css
h1 {
 font-size: 2.5em; /* 40px/16=2.5em */
}

h2 {
 font-size: 1.875em; /* 30px/16=1.875em */
}

p {
 font-size: 0.875em; /* 14px/16=0.875em */
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_font-size_em)

위의 예에서 em의 텍스트 크기는 이전 예와 동일하다. 그러나 em 크기를 사용하면 모든 브라우저에서 텍스트 크기를 조정할 수 있다. 하지만 불행하게도 이전 버전의 IE에는 여전히 문제가 있다. 텍스트는 크게 만들 때 보다 커지고 작아질 때 보다 작아진다.

------

## Use a Combination of Percent and Em

모든 브라우저에서 작동하게 하는 솔루션은 `<body>`요소의 기본 글꼴 크기를 백분율로 설정하는 것이다.

### 예제

```css
body {
 font-size: 100%;
}

h1 {
 font-size: 2.5em;
}

h2 {
 font-size: 1.875em;
}

p {
 font-size: 0.875em;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_font-size_percent_em)

우리의 코드는 이제 훌륭하게 작동한다! 모든 브라우저에서 동일한 텍스트 크기를 표시하며 모든 브라우저가 텍스트를 확대하거나 크기를 조정할 수 있다.

------

## Font Weight

The `font-weight` property specifies the weight of a font:

### 예제

```css
p.normal {
 font-weight: normal;
}

p.thick {
 font-weight: bold;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_font-weight)

------

## Responsive Font Size

텍스트 크기는 "vw"단위로 설정될 수 있으며 "뷰포트 너비"를 의미한다.

이렇게하면 텍스트 크기가 브라우저 창의 크기를 따른다.

# Hello World

글꼴 크기가 어떻게 조정되는지 보려면 브라우저 창의 크기를 조정하면 된다.

### 예제

```html
<h1 style="**font-size:10vw**">Hello World</h1>
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_font_responsive)

뷰포트는 브라우저 창 크기이고 1vw = 뷰포트 너비의 1%이다.

만약 뷰포트가 50cm 인경우에는 1vw는 0.5cm이다.

------

## Font Variant

`font-variant`속성은 텍스트를 작은 대문자로 표시할지의 여부를 지정한다.

작은 대문자 글꼴에서는 모든 소문자가 대문자로 변환된다. 그러나 변환된 대문자는 텍스트의 원래 대문자보다 작은 글꼴 크기로 나타난다.

### 예제

```css
p.normal {
 font-variant: normal;
}

p.small {
 font-variant: small-caps;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_font-variant)

------

## All CSS Font Properties

| 속성                                                         | 설명                                             |
| :----------------------------------------------------------- | :----------------------------------------------- |
| [font](https://www.w3schools.com/cssref/pr_font_font.asp)    | 하나의 선언으로 폰트속성을 셋팅한다.             |
| [font-family](https://www.w3schools.com/cssref/pr_font_font-family.asp) | 텍스트의 폰트패밀리를 정의한다.                  |
| [font-size](https://www.w3schools.com/cssref/pr_font_font-size.asp) | 텍스트의 폰트크기를 정한다.                      |
| [font-style](https://www.w3schools.com/cssref/pr_font_font-style.asp) | 텍스트의 폰트스타일을 정한다.                    |
| [font-variant](https://www.w3schools.com/cssref/pr_font_font-variant.asp) | 텍스트를 작은 대문자로 표시할지 여부를 지정한다. |
| [font-weight](https://www.w3schools.com/cssref/pr_font_weight.asp) | 폰트의 크기를 정한다.                            |

[CSS Icons](./CSS_icons.md)

