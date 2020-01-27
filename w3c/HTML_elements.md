# HTML Elements

## HTML Elements

HTML원소들은 보통 시작태그와 끝태그로 구성되어있습니다. 그리고 그 사이에 내용이 들어갑니다.

> <tagname>내용은 여기에..</tagname>

HTML element는 start태그에서 end tag로 까지의 모든것을 말합니다.

```HTML
<p>My first paragraph.</p>
```

| Start tag | Element content     | End tag |
| :-------- | :------------------ | :------ |
| <h1>      | My First Heading    | </h1>   |
| <p>       | My first paragraph. | </p>    |
| <br>      |                     |         |

내용이없는 HTML 요소를 빈 엘리먼트라고합니다.

 빈 엘리먼트에는 `<br>` 엘리먼트 (줄 바꿈을 나타냄)와 같이 종료 태그가 없습니다.



## 중첩된 HTML Elements

HTML 엘리먼트들은 중첩될 수 있습니다. ( 엘리먼트들은 엘리먼트에 포함될 수 있습니다.)

모든 HTML 문서들은 중첩된 HTML엘리먼트들로 구성되어 있습니다.

아래 예제는 4가지의 HTML 엘리먼트들로 구성되어 있습니다.



### 예제

```html
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```



### 예제설명

 `<html>` 엘리먼트는 **전체 문서**를 정의합니다.

이것은 **시작** 태그 `<html>`과  **끝** 태그 `</html>`을 가지고 있습니다.

`<html>` 태그 안에는 `<body>` 엘리먼트가 있습니다.

```html
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```

 `<body>` 엘리먼트는 **문서의 몸체**를 정의합니다.

이것은 시작태그 `<body>`와 끝태그 `</body>`를 가집니다.

`<body>` 엘리먼트 안에는 두가지의 다른 HTML 엘리먼트들이 있습니다 : `<h1>`  과 `<p>`

```html
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
```

`<h1>` 엘리먼트는 **헤딩**을 말합니다.

이것은 시작태그 `<h1>` 과 끝 태그 `</h1>`으로 구성되어 있습니다.

이 엘리먼트 내용은 My First Heading 입니다.

```php+HTML
<h1>My First Heading</h1>
```

<p> 태그는 단락을 말합니다.

이것은 시작태그 `<p>`와 끝 태그 `</p>`로 구성되어 있습니다.

이 엘리먼트 내용은 My first paragraph 입니다.

```html
<p>My first paragraph.</p>
```



## 끝 태그를 잊지마세요!

몇몇 HTML 엘리먼트들은 올바르게 보여질지도 모르지만 이것에 안주하지 마세요

### 예제

```html
<html>
<body>

<p>This is a paragraph
<p>This is a paragraph

</body>
</html>
```

이 예제는 모든 브라우저에서 잘 작동합니다. 왜냐하면 닫는 태그가 옵션이기 때문이죠

**이것에 안주하지 마세요. 만약 당신이 끝 태그를 잊어버린다면 기대하지않는 에러가 발생할수도 있습니다.**



## 빈 HTML Elements

HTML 엘리먼트에서 내용이 없는 엘리먼트를 empty element 라고 부릅니다.

` <br>` 태그는 닫는 태그가 없는 빈 엘리먼트 태그입니다.(이 태그는 다음줄로 넘어가게 해줍니다.)

### 예제

```html
<p>This is a <br> paragraph with a line break.</p>
```

빈 태그는 `<br />`과 같이 여는 태그에서 "닫힐"수 있습니다.

HTML5는 빈 요소를 닫을 필요가 없습니다. 

그러나보다 엄격한 유효성 검사를 원하거나 XML 파서가 문서를 읽을 수있게하려면 모든 HTML 요소를 올바르게 닫아야합니다.

## HTML 은 대문자와 소문자에 민감하지 않습니다.

HTML 태그는 대소 문자를 구분하지 않습니다. `<P>`는 `<p>`와 동일합니다.

HTML5 표준에는 소문자 태그가 필요하지 않지만 W3C는 HTML에서 소문자를 권장하며 XHTML과 같은보다 엄격한 문서 유형에는 소문자를 요구합니다.

[HTML 속성들](./HTML_attributes.md)

