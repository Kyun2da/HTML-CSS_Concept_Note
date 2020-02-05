# HTML Computer Code Elements

### Computer Code

```html
<code>
    x = 5;<br>
    y = 6;<br>
    z = x + y;
</code>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_formatting_intro3)

------

## HTML `<kbd>` For Keyboard Input

HTML `<kbd>` 엘리먼트는 유저의 키보드 입력이나 소리 입력과 같은 유저의 입력을 의미한다.

텍스트는 `<kbd>`태그로 둘러쌓여 있고 전형적으로 모노스페이스 폰트로 보여진다

### 예제

```html
<p>Save the document by pressing <kbd>Ctrl + S</kbd></p>
```

결과:

컨트롤s를 누르면 문서가 저장된다.

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_formatting_kbd)

------

## HTML `<samp>` For Program Output

`<samp>`엘리먼트는 프로그램이나 컴퓨터 시스템으로부터의 출력을 의미한다.

텍스트는 `<samp>`태그에 의해 모노스페이스 폰트로 보여진다.

### 예제

```html
<p>If you input wrong value, the program will return <samp>Error!</samp></p>
```

결과:

If you input wrong value, the program will return Error!

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_formatting_samp)

## HTML `<code>` For Computer Code

HTML `<code>`엘리먼트는 컴퓨터 코드의 프래그먼트를 정의한다.

텍스트는 모노스페이스 폰트로 `<code>`태그에 의해 보여진다.

### 예제

```html
<code>x = 5;y = 6;z = x + y;</code>
```

Result:

`x = 5; y = 6; z = x + y;`

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_formatting_code)

`<code>` 요소는 여분의 공백과 줄 바꿈을 유지하지 않는다.  이 문제를 해결하기 위해 `<code>` 요소를 `<pre>`요소 안에 넣을 수 있다.

### 예제

<pre><code>x = 5;y = 6;z = x + y;</code></pre>

Result:

`x = 5; y = 6; z = x + y;`

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_formatting_codepre)

------

## HTML `<var>` For Variables

HTML <var> 요소는 변수를 정의한다.

변수는 수학 표현식의 변수이거나 프로그래밍 컨텍스트의 변수 일 수 있다.

### 예제

Einstein wrote: <var>E</var> = <var>mc</var><sup>2</sup>.

Result:

Einstein wrote: E = mc2.

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_formatting_var)

------

## HTML Computer Code Elements

| 태그                                                    | 설명                             |
| :------------------------------------------------------ | :------------------------------- |
| [`<code>`](https://www.w3schools.com/tags/tag_code.asp) | 프로그래밍 코드를 정의한다.      |
| [`<kbd>`](https://www.w3schools.com/tags/tag_kbd.asp)   | 키보드 인풋을 정의한다.          |
| [`<samp>`](https://www.w3schools.com/tags/tag_samp.asp) | 컴퓨터 출력을 정의한다           |
| [`<var>`](https://www.w3schools.com/tags/tag_var.asp)   | 변수를 정의한다                  |
| [`<pre>`](https://www.w3schools.com/tags/tag_pre.asp)   | 미리 포맷팅된 텍스트를 정의한다. |

[HTML Forms](./HTML_forms.md)