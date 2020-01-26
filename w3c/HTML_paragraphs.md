# HTML Paragraphs

## HTML Paragraphs

HTML의 `<p>`엘리먼트는 단락으로 정의됩니다.

### 예제

```html
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
```



## HTML 보여주기

당신은 어떻게 HTML이 보여질지 확신할 수 없습니다.

크거나 작은 스크린에서 그리고 재 조정된 윈도우에서 다른 결과를 만들어낼 것입니다.

HTML에서 당신은 결과를 당신의 HTML코드안에  추가적인 라인이나 공간을 추가함으로써 바꿀 수 없습니다. 

이 브라우저는 페이지가 보여질 때 추가적인 공간과 추가적인 라인을 제거할 것입니다.

### 예제

```html
<p>
This paragraph
contains a lot of lines
in the source code,
but the browserignores it.
</p>
<p>This paragraphcontains         a lot of spaces
in the source         code,
but the        browser
ignores it.
</p>
```





## 끝 태그를 잊지 마세요

대부분의 브라우저는 당신이 끝태그를 까먹었을지라도 올바르게 작성할지도 모릅니다.

### 예제

```html
<p>This is a paragraph.<p>This is another paragraph.
```

이 예제는 모든 브라우저에 작동합니다. 하지만 이것에 의존하지 마세요.

언젠가 에러를 발생할지도 모르기 때문입니다.



## HTML 라인 깨기

 HTML ` <br>` 엘리먼트는 다음 라인으로 이동합니다.

`<br> ` 만약 당신이 새로운 단락을 시작하지 않고 새로운 라인을 원하면 br을 사용하세요.

### 예제

```html
<p>This is<br>a paragraph<br>with line breaks.</p>
```



## HTML `<pre>` 엘리먼트

HTML `<pre>` 엘리먼트는 사전 형식화 된 텍스트를 정의합니다.

`<pre>` 요소 안의 텍스트는 고정 너비 글꼴 (일반적으로 Courier)로 표시되며 공백과 줄 바꿈을 모두 유지합니다.

### 예제

```html
<pre>  
My Bonnie lies over the ocean. 

My Bonnie lies over the sea.  

My Bonnie lies over the ocean.  

Oh, bring back my Bonnie to me.
</pre>
```



## HTML Tag 레퍼런스

W3Schools의 태그 레퍼런스는 HTML 엘리먼트와 그것들의 속성에 관해 추가적인 정보를 포함합니다.

| 태그    | 설명                               |
| :------ | :--------------------------------- |
| `<p>`   | 단락을 정의합니다.                 |
| `<br>`  | 하나의 라인을 삽입합니다.          |
| `<pre>` | 미리 포맷팅된 텍스트를 정의합니다. |



[HTML Styles](./w3c/HTML_styles.md)













