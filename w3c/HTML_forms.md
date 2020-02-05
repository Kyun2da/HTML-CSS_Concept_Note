# HTML Forms

## The `<form>` Element

HTML `<form>`엘리먼트는 유저인풋을 수집하기 위해 폼을 사용하는데에 사용한다.

```html
<form>
.
*form elements*
.
</form>
```

HTML 폼은 form 엘리먼트를 포함한다.

폼 엘리먼트는 인풋 엘리먼트의 텍스트 필드, 체크박스, 라디오버튼, 제출버튼, 등등의 다른 타입이 될 수 있다.

------

## The `<input>` Element

`<input>`엘리먼트는 폼 엘리먼트에서 가장 중요한 엘리먼트이다.

`<input>`엘리먼트는 몇가지 방식으로 보여질 수 있고 타입 속성에 따라 달려있다.

| 타입                    | 설명                           |
| :---------------------- | :----------------------------- |
| `<input type="text">`   | 하나의 텍스트 필드를 정의한다. |
| `<input type="radio">`  | 하나의 라디오 버튼을 정의한다. |
| `<input type="submit">` | 하나의 제출버튼을 정의한다.    |

너는 더많은 인풋 타입을 이 튜토리얼에서 배울 것 이다.

------

## Text Input

`<input type="text">` 는 텍스트 인풋의 필드에 대한 하나의 라인을 정의한다.

### Example

```html
<form>
 First name:<br>
 <input type="text" name="firstname"><br>
 Last name:<br>
 <input type="text" name="lastname">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_form_text)

**Note:** 폼 그자체는 보이지 않는다. 또한 텍스트필드의 기본 넓이는 20개의 문자가 들어갈 넓이라는 것을 기억해라

------

## Radio Button Input

`<input type="radio">` 는 라디오 버튼을 정의한다.

라디오버튼은 제한된 선택의 수중 하나의 선택을 유저에게 하도록하는 버튼이다.

### 예제

```html
<form>
 <input type="radio" name="gender" value="male" checked> Male<br>
 <input type="radio" name="gender" value="female"> Female<br>
 <input type="radio" name="gender" value="other"> Other
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_form_radio)

------

## The Submit Button

`<input type="submit">`은 폼을 다루는 폼 데이터에 제출할때 쓰이는 버튼이다.

폼핸들러는 일반적으로 처리데는 인풋데이터를 위해 있는 서버페이지를 의미한다.

폼핸들러는 폼의 액션 속성에서 정할 수 있다.

### 예제

```html
<form action="/action_page.php">
 First name:<br>
 <input type="text" name="firstname" value="Mickey"><br>
 Last name:<br>
 <input type="text" name="lastname" value="Mouse"><br><br>
 <input type="submit" value="Submit">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_form_submit)

------

## The Action Attribute

액션 속성은 폼이 제출 되었을 때 행동하게 되는 액션을 정의한다.

일반적으로 폼데이터는 유저가 submit 버튼을 누를 때 웹페이지의 서버에 보내진다.

위의 예제에서 폼데이터는 "/action_page.php" 이라고 불리는 서버페이지에 보내지게 된다. 이 페이지는 폼데이터를 다루는 서버쪽 스크립트가 보함되어있는 페이지이다.

```html
<form action="/action_page.php">
```

If the `action` attribute is omitted, the action is set to the current page.

------

## The Target Attribute

타겟 속성은 만약 제출된 결과가 새로운 브라우저 탭에서 열릴지, 프레임에서 열릴지, 현재 윈도우에서 열릴지를 결정하는 속성이다.

기본값은 `_self`이고 이것은 제출된 폼이 현재페이지에서 열리는 것을 의미한다.

새로운 탭에서 결과를 열고 싶다면 `_blank`값을 사용하면 된다.

### 예제

```html
<form action="/action_page.php" target="_blank">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_form_target)

------

## The Method Attribute

`method`속성은 HTTP 메소드인데 폼데이터를 제출할때 사용되는 방법을 의미한다.(GET 과 POST 방식이 있음)

### 예제

```html
<form action="/action_page.php" method="get">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_form_get)

or:

### 예제

```html
<form action="/action_page.php" method="post">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_form_post)

------

## When to Use GET?

기본 방식은 GET방식이다.

그러나 get을 사용하면 제출된 데이터가 주소창에 보이게 되는 방식이 될 것이다.

```
/action_page.php?firstname=Mickey&lastname=Mouse
```

**Notes on GET:**

- 이름 / 값 쌍으로 양식 데이터를 URL에 추가
- URL의 길이는 제한되어 있다 (2048 자)
- 민감한 데이터를 보내려면 절대 GET을 사용하지 말것 (URL에서 볼 수 있다)
- 사용자가 결과를 즐겨 찾기에 추가하려는 양식 제출에 유용
- GET은 Google의 쿼리 문자열과 같은 비보안 데이터에 적합

------

## When to Use POST?

양식 데이터에 민감한 정보 나 개인 정보가 포함 된 경우 항상 POST를 사용하자. POST 메소드는 제출 된 양식 데이터를 페이지 주소 필드에 표시하지 않는다.

**Notes on POST:**

- POST에는 크기 제한이 없으며 대량의 데이터를 보내는 데 사용할 수 있다.
- POST를 통한 양식 제출은 북마크 할 수 없다

------

## The Name Attribute

각 입력 필드에는 제출할`name` 속성이 있어야한다.

`name` 속성이 생략되면 해당 입력 필드의 데이터가 전혀 전송되지 않는다.

이 예에서는 "성"입력 필드 만 제출하게된다.

### 예제

```html
<form action="/action_page.php">
 First name:<br>
 <input type="text" value="Mickey"><br>
 Last name:<br>
 <input type="text" name="lastname" value="Mouse"><br><br>
 <input type="submit" value="Submit">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_form_submit_id)

------

## Grouping Form Data with `<fieldset>`

`<fieldset>` 요소는 관련 데이터를 양식으로 그룹화하는 데 사용된다.

`<legend>` 요소는 `<fieldset>` 요소의 캡션을 정의한다.

### 예제

```html
<form action="/action_page.php">
 <fieldset>
  <legend>Personal information:</legend>
  First name:<br>
  <input type="text" name="firstname" value="Mickey"><br>
  Last name:<br>
  <input type="text" name="lastname" value="Mouse"><br><br>
  <input type="submit" value="Submit">
 </fieldset>
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_form_legend)

------

아래에 모든 `<form>`속성이 있다.

| Attribute      | Description                                                  |
| :------------- | :----------------------------------------------------------- |
| accept-charset | 제출 된 양식에 사용 된 문자 세트를 지정합니다 (기본값 : 페이지 문자 세트). |
| action         | 양식을 제출할 주소 (URL)를 지정합니다 (기본값 : 제출 페이지). |
| autocomplete   | 브라우저가 양식을 자동 완성해야하는지 여부를 지정합니다 (기본값 : on). |
| enctype        | 제출 된 데이터의 인코딩을 지정합니다 (기본값 : URL 인코딩 됨). |
| method         | 양식을 제출할 때 사용되는 HTTP 메소드를 지정합니다 (기본값 : GET). |
| name           | 양식을 식별하는 데 사용되는 이름을 지정합니다 (DOM 사용법의 경우 : document.forms.name). |
| novalidate     | 브라우저가 양식의 유효성을 검사하지 않도록 지정합니다.       |
| target         | 조치 속성에서 주소의 대상을 지정합니다 (기본값 : _self).     |

[HTML Form Elements](./HTML_formelements.md)