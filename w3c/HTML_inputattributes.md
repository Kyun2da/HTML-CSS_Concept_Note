# HTML Input Attributes

## The value Attribute

`value`속성은 인풋필드에 초기값으로 정해 놓을 수 있다.

### 예제

```html
<form action="">
 First name:<br>
 <input type="text" name="firstname" value="John">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_attributes_value)

------

## 읽기만 가능한 속성

`readonly`속성은 인풋필드가 오직 읽을 수 만 있도록 바꾼다.

### 예제

```html
<form action="">
 First name:<br>
 <input type="text" name="firstname" value="John" readonly>
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_attributes_readonly)

------

## 비활성화 속성

`disabled`속성은 인풋필드를 비활성화 시킬 수 있도록 해준다.

### 예제

```html
<form action="">
 First name:<br>
 <input type="text" name="firstname" value="John" disabled>
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_attributes_disabled)

------

## The size Attribute

`size`속성은 인풋필드의 상자 크기를 정하는 속성이다(들어갈 수 있는 문자의 개수로 크기를 정함)

### 예제

```html
<form action="">
 First name:<br>
 <input type="text" name="firstname" value="John" size="40">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_attributes_size)

------

## The maxlength Attribute

`maxlength`속성은 인풋필드의 길이의 최대를 제한해준다.

### 예제

```html
<form action="">
 First name:<br>
 <input type="text" name="firstname" maxlength="10">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_attributes_maxlength)

`maxlength`속성에서 인풋필드는 문자의 개수보다 더 받아들여질 수 없다.

`maxlength`속성은 어떠한 피드백도 제공하지않는다. 만약 너가 유저에게 알람을 보여주고 싶다면 너는 자바스크립트 코드를 작성해야만 한다.

**Note:** 입력 제한은 완전하지 않으며 JavaScript는 잘못된 입력을 추가하는 여러 가지 방법을 제공한다. 입력을 안전하게 제한하려면 수신기 (서버)에서도 입력을 확인해야한다!

------

## HTML5 속성

HTML5의 `<input>`속성은 다음과 같은 속성을 허용한다.

- autocomplete
- autofocus
- form
- formaction
- formenctype
- formmethod
- formnovalidate
- formtarget
- height and width
- list
- min and max
- multiple
- pattern (regexp)
- placeholder
- required
- step

그리고 `<form>`속성에는 다음과 같은 속성을 허용한다.

- autocomplete
- novalidate

------

## The autocomplete Attribute

`autocomplete` 속성은 폼이나 인풋필드가 자동완성을 키거나 끌지를 결정하는 속성이다.

자동완성기능이 켜지면 브라우저는 자동적으로 유저가 전에 완성한 유저의 값을 기준으로 인풋값을 완성시켜주는 기능이다.

**Tip:** 양식에 대해 자동 완성 "on"을, 특정 입력 필드에 대해 "off"를 가질 수 있으며, 그 반대도 가능하다.

`autocomplete` 속성은 텍스트, 검색, URL, 전화, 이메일, 비밀번호, 날짜 선택기, 범위 및 색상 유형과 함께 ''`<form>` 및 `<input>` 유형에서 작동한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

자동완성기능이 켜진 HTML 폼의 예시이다.

```html
<form action="/action_page.php" autocomplete="on">
 First name:<input type="text" name="fname"><br>
 Last name: <input type="text" name="lname"><br>
 E-mail: <input type="email" name="email" autocomplete="off"><br>
 <input type="submit">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_autocomplete)

**Tip:** 몇몇 브라우저에서는 이것을 작동시키기 위해 자동완성기능을 켜야할 필요가 있을지도 모른다.

------

## The novalidate Attribute

`<novalidate>`속성은 `<form>`속성이다.

존재하는 경우, novalidate는 제출할 때 양식 데이터를 유효성 검증하지 않도록 지정한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

제출될때 폼이 타당한지 검사할 필요가 없다.

```html
<form action="/action_page.php" novalidate>
 E-mail: <input type="email" name="user_email">
 <input type="submit">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_form_novalidate)

------

## The autofocus Attribute

`autofocus`속성은 인풋필드가 자동적으로 페이지가 로드될때 focus된다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

First name인풋 필드가 자동적으로 페이지가 로드되면 focus 된다.

```html
First name:<input type="text" name="fname" autofocus>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_autofocus)

------

## The form Attribute

`form`속성은 `<input>` 엘리먼트가 속하는 하나 이상의 양식을 지정한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

하나의 인풋필드가 폼 밖에 위치하고 있음(그러나 여전히 폼의 부분임)

```html
<form action="/action_page.php" id="form1">
 First name: <input type="text" name="fname"><br>
 <input type="submit" value="Submit">
</form>

Last name: <input type="text" name="lname" form="form1">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_form)

------

## The formaction Attribute

formaction 속성은 양식이 제출 될 때 입력 제어를 처리 할 파일의 URL을 지정한다.

`formaction`속성은 `form`엘리먼트의 액션속성을 상속한다.

`formaction`속성은 `type="submit"`과 `type="image"`와 사용된다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

두개의 다른 제출버튼이 있는 HTML 폼은 각각 다른 역할을 한다.

```html
<form action="/action_page.php">
 First name: <input type="text" name="fname"><br>
 Last name: <input type="text" name="lname"><br>
 <input type="submit" value="Submit"><br>
 <input type="submit" formaction="/action_page2.php"
 value="Submit as admin">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_formaction)

------

## The formenctype Attribute

`formenctype` 속성은 제출시 양식 데이터를 인코딩하는 방법을 지정한다. (method = "post"인 양식에만 해당).

`formenctype` 속성은 `<form>` 요소의 enctype 속성보다 우선시된다.

`formenctype`속성은 `type="submit"`과 `type="image"`와 함께 사용된다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

기본적으로 인코딩되어 있고 (첫 번째 제출 버튼) "multipart / form-data"(두 번째 제출 버튼)로 인코딩 된 양식 데이터를 보낸다.

```html
<form action="/action_page_binary.asp" method="post">
 First name: <input type="text" name="fname"><br>
 <input type="submit" value="Submit">
 <input type="submit" formenctype="multipart/form-data"
 value="Submit as Multipart/form-data">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_formenctype)

------

## The formmethod Attribute

`formmethod`속성은 양식 데이터를 조치 URL로 전송하기위한 HTTP 메소드를 정의한다.

`formmethod` 속성은 `<form>` 요소의 method 속성보다 우선시된다.

`formmethod` 속성은 `type = "submit"`및 `type = "image"`와 함께 사용할 수 있습니다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

두 번째 제출 단추는 다음 양식의 HTTP 메소드를 대체한다.

```html
<form action="/action_page.php" method="get">
 First name: <input type="text" name="fname"><br>
 Last name: <input type="text" name="lname"><br>
 <input type="submit" value="Submit">
 <input type="submit" formmethod="post" value="Submit using POST">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_formmethod)

------

## The formnovalidate Attribute

`formnovalidate` 속성은 `<form>` 요소의 `novalidate` 속성을 대체한다.

`formnovalidate` 속성은 `type = "submit"`과 함께 사용할 수 있다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

두개의 제출버튼이 있는 폼(하나는 유효성검사가 있고 다른 하나는 없다.)

```html
<form action="/action_page.php">
 E-mail: <input type="email" name="userid"><br>
 <input type="submit" value="Submit"><br>
 <input type="submit" formnovalidate value="Submit without validation">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_formnovalidate)

------

## The formtarget Attribute

`formtarget` 속성은 양식을 제출 한 후 수신 된 응답을 표시 할 위치를 나타내는 이름 또는 키워드를 지정한다.

`formtarget` 속성은`<form>`엘리먼트의 target 속성보다 우선시된다.

`formtarget` 속성은`type = "submit"` 및 `type = "image"`와 함께 사용할 수 있다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

두개의 제출버튼 이있지만 두개는 다른 타겟 윈도우를 가리킨다.

```html
<form action="/action_page.php">
 First name: <input type="text" name="fname"><br>
 Last name: <input type="text" name="lname"><br>
 <input type="submit" value="Submit as normal">
 <input type="submit" formtarget="_blank"
 value="Submit to a new window">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_formtarget)

------

## The height and width Attributes

높이 및 너비 속성은 `<input type = "image">` 요소의 높이와 너비를 지정한다.

항상 이미지 크기를 지정해라. 브라우저가 크기를 모르면 이미지가로드되는 동안 페이지가 깜박인다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

제출버튼으로 이미지를 정의하고 높이와 넓이 속성을 제어한다.

```html
<input type="image" src="img_submit.gif" alt="Submit" width="48" height="48">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_height_width)

------

## The list Attribute

list 속성은 `<input>` 요소에 대해 사전 정의 된 옵션이 포함 된 `<datalist>` 요소를 나타낸다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/incompatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

`<datalist>`에 사전 정의 된 값이있는 `<input>` 요소 :

```html
<input list="browsers">

<datalist id="browsers">
 <option value="Internet Explorer">
 <option value="Firefox">
 <option value="Chrome">
 <option value="Opera">
 <option value="Safari">
</datalist>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_datalist)

------

## The min and max Attributes

최소 및 최대 속성은 `<input>` 요소의 최소 및 최대 값을 지정한다.

최소 및 최대 속성은 숫자, 범위, 날짜, 날짜 / 시간, 월, 시간 및 주와 같은 입력 유형에서 작동한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<input> elements with min and max values:

Enter a date before 1980-01-01:
<input type="date" name="bday" max="1979-12-31">

Enter a date after 2000-01-01:
<input type="date" name="bday" min="2000-01-02">

Quantity (between 1 and 5):
<input type="number" name="quantity" min="1" max="5">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_max_min)

------

## The multiple Attribute

multiple 속성은 사용자가 `<input>` 요소에 둘 이상의 값을 입력 할 수 있도록 지정한다.

multiple 속성은 email 및 file 입력 유형과 함께 작동한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

파일업로드 칸에는 다중 값이 될 수 있다.

```html
Select images: <input type="file" name="img" multiple>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_multiple)

------

## The pattern Attribute

pattern 속성은 `<input>` 요소의 값을 검사 할 정규식을 지정한다.

pattern 속성은 text, search, url, tel, email 및 password 입력 유형과 함께 작동한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

인풋필드는 오직 세글자만 될 수 있다.(숫자도 안되고 특수문자도 안된다.)

```html
Country code: <input type="text" name="country_code" pattern="[A-Za-z]{3}" title="Three letter country code">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_pattern)

------

## The placeholder Attribute

'placeholder'속성은 입력 필드의 예상 값 (샘플 값 또는 형식에 대한 간단한 설명)을 설명하는 힌트를 지정한다.

힌트는 사용자가 값을 입력하기 전에 입력 필드에 표시된다.

'placeholder'속성은 text, search, url, tel, email 및 password와 같은 입력 유형에서 작동한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

힌트가 있는 인풋이다.

```html
<input type="text" name="fname" placeholder="First name">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_placeholder)

------

## The required Attribute

`required` 속성은 양식을 제출하기 전에 입력 필드를 채워야 함을 지정한다.

'필수'속성은 텍스트, 검색, URL, 전화, 이메일, 비밀번호, 날짜 선택기, 번호, 확인란, 라디오 및 파일과 같은 입력 유형에서 작동한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

인풋필드에 값을 넣어야 제출할 수 있다.

```html
Username: <input type="text" name="usrname" required>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_required)

------

## The step Attribute

`step` 속성은`<input>`엘리먼트의 유효한 숫자 간격을 지정한다.

예 : step = "3"인 경우 유효한 숫자는 -3, 0, 3, 6 등이 될 수 있다.

**Tip:** step 속성을 max 및 min 속성과 함께 사용하여 다양한 유효한 값을 만들 수 있다.

step 속성은 숫자, 범위, 날짜, 날짜 / 시간, 월, 시간 및 주와 같은 입력 유형에서 작동한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

숫자 간격이 있는 인풋 태그

```html
<input type="number" name="points" step="3">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_step)

------

## HTML Form and Input Elements

| 태그                                                      | 설명                                 |
| :-------------------------------------------------------- | :----------------------------------- |
| [`<form>`](https://www.w3schools.com/tags/tag_form.asp)   | 유저 인풋에 대한 HTML 폼을 정의한다. |
| [`<input>`](https://www.w3schools.com/tags/tag_input.asp) | 인풋을 정의한다.                     |