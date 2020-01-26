# HTML 이란?

HTML은 웹페이지를 만드는데 쓰이는 표준 마크업 언어입니다.

- HTML은 Hyper Text Markup Language의 약자입니다.
- HTMl은 웹페이지의 구조를 묘사합니다.
- HTML은 원소들의 묶음으로 구성됩니다.
- HTML 원소들은 브라우저에게 어떻게 내용을 보여줄지 말해줍니다.
- HTML 원소들은 태그로 대표됩니다.
- HTML 태그들은 "heading", "paragraph", "table", 기타 등등의 내용들의 라벨을 붙입니다.
- 브라우저는 HTML태그를 표시하지 않지만 이를 사용하여 페이지의 내용을 렌더링합니다.

# 간단한 HTML 문서 예제

```html
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```

### 예제 설명

- `<!DOCTYPE html>` : 문서가 HTML5가 될 수 있도록 정의하여 선언하는 태그
- `html` : 이 원소는 HTML페이지의 루트 원소입니다.
- `head` : 이 원소는 문서에 관한 메타 정보를 포함합니다.
- `title` : 제목 원소는 문서의 제목에 특화되어 있습니다.
- `body` : 이 원소는 페이지에 보여지는 내용을 포함합니다.
- `h1` : 이 원소는 큰 헤딩을 말합니다.
- `p` : 이 원소는 단락을 정의합니다.

## HTML 태그

HTML 태그는 각 묶음에의해 둘러싸입니다.

> <tagname> 내용은 이 곳에 둘러싸입니다...</tagname>

-  HTML태그는 일반적으로  **짝으로** 둘러싸입니다. 이를테면 <p>와 </p>처럼 말이죠.
- 첫 번째 태그는  **start tag(시작 태그),** 라고 하고 두 번째 태그는 **end tag(끝 태그)**라고 합니다.
- 끝 태그는 스타트태그 처럼 쓰이지만, 그러나 태그의 이름 **앞에 슬래시**가 와야합니다.

## 웹 브라우저

웹브라우저의 목적은 HTML문서를 읽고 그것들을 보여주는데에 있습니다.

브라우저는 HTML태그를 보여주지는 않지만 그것들을 이용해 어떻게 문서를 보여줄지를 결정합니다.

## The <!DOCTYPE> 선언

`<!DOCTYPE>` 선언은 문서타입을 대표하고, 브라우저가 웹페이지를 똑바로 보여줄 수 있도록 도와줍니다.

이것은 오직 (HTML태그 이전)페이지 상단에 한번만 나타나야합니다.

 `<!DOCTYPE>`  선언은 민감한 케이스가 아닙니다.

HTML을 위한 `<!DOCTYPE>`  선언은

```html
<!DOCTYPE html>
```

이라고 합니다.

## HTML 버전

웹의 초기때부터 많은 HTML 버전들이 있었습니다.

| Version   | Year |
| :-------- | :--- |
| HTML      | 1991 |
| HTML 2.0  | 1995 |
| HTML 3.2  | 1997 |
| HTML 4.01 | 1999 |
| XHTML     | 2000 |
| HTML5     | 2014 |

[HTML 기본예제들로 가기](./w3c/HTML_basic.md)