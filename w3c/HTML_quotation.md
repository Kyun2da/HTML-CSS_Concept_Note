# HTML Quotation and Citation Elements

## HTML `<q>` 짧은 인용구를위함

 HTML `<q>` 엘리먼트는 짧은 인용구를 정의합니다.

브라우저는 일반적으로  `<q>` 엘리먼트로 쿼테이션 마스를 삽입합니다.

### Example

```html
<p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>
```



------

## HTML `<blockquote>` 블록 쿼트

HTML 은 블록 쿼테이트를 넣기위해 `<blockquote>` 를 사용합니다. 이는 문장에 블록을 넣어 다른 문장과 구분되게 보이게 합니다.

### 예제

```html
<p>Here is a quote from WWF's website:</p><blockquote cite="http://www.worldwildlife.org/who/index.html">For 50 years, WWF has been protecting the future of nature.The world's leading conservation organization,WWF works in 100 countries and is supported by1.2 million members in the United States andclose to 5 million globally.</blockquote>
```



## HTML `<abbr>` 축약을위함

HTML `<abbr>` 엘리먼트는 축약을위한 마크 입니다. 축약을 마킹하는 것은  번역 시스템과 서치엔진같은 브라우저에게 유용한 정보를 줍니다.

### 예제

```html
<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
```



------

## HTML `<address>` for Contact Information

HTML `<address>` 엘리먼트는 연락 정보를 정의합니다.

`<address>` 엘리먼트는 종종 이탤릭 체로 보여지고 대부분의 브라우저는  그전과 그위에 라인을 추가합니다 

### 예제

```html
<address>
Written by John Doe.<br>
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>
```



------

## HTML `<cite>` 작품 제목을 위함

HTML 엘리먼트 `<cite>`는 작품 제목을 위한 엘리먼트 입니다.

브라우저는 종종 `<cite>` 를 이탤릭 체로 정의합니다.

### 예제

```html
<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>
```



------

## HTML `<bdo>` 

HTML `<bdo>` 엘리먼트는 방향을 바꿔서 보여줍니다.

`<bdo>` 엘리먼트는 텍스트의 방향을 바꿔서 보여줍니다. 이를테면 left 를 tfel 로 보여줄 것입니다.

### 예제

```html
<bdo dir="rtl">This text will be written from right to left</bdo>
```

[HTML_comments](/w3c/HTML_comments.md)