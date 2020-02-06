# HTML Input Types

이 챕터는 `<input>`엘리먼트에 대해서 다른 인풋 타입을 묘사한다.

------

## HTML Input Types

HTML에서 너가 사용할 수있는 인풋타입들이 아래에 있다.

- `<input type="button">`
- `<input type="checkbox">`
- `<input type="color">`
- `<input type="date">`
- `<input type="datetime-local">`
- `<input type="email">`
- `<input type="file">`
- `<input type="hidden">`
- `<input type="image">`
- `<input type="month">`
- `<input type="number">`
- `<input type="password">`
- `<input type="radio">`
- `<input type="range">`
- `<input type="reset">`
- `<input type="search">`
- `<input type="submit">`
- `<input type="tel">`
- `<input type="text">`
- `<input type="time">`
- `<input type="url">`
- `<input type="week">`

------

## Input Type Text

`<input type="text">`는 하나의 텍스트 인풋 필드를 정의한다.

### 예제

```html
<form>
 First name:<br>
 <input type="text" name="firstname"><br>
 Last name:<br>
 <input type="text" name="lastname">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_text)

------

## Input Type Password

`<input type="password">`는 패스워드 필드를 정의한다.

### 예제

```html
<form>
 User name:<br>
 <input type="text" name="username"><br>
 User password:<br>
 <input type="password" name="psw">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_password)

## Input Type Submit

`<input type="submit">`은 폼핸들러에게 폼데이터를 제출하는 버튼이다.

폼핸들러는 일반적으로 인풋데이터를 처리하는 스크립트로 되어있는 서버페이지이다.

폼 핸들러는 폼의 액션설정에 특화되어 있다.

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

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_submit)

만약 너가 제출 버튼의 값속성을 생략한다면 그 버튼은 기본값으로 텍스트를 얻을 것이다.

### 예제

```html
<form action="/action_page.php">
 First name:<br>
 <input type="text" name="firstname" value="Mickey"><br>
 Last name:<br>
 <input type="text" name="lastname" value="Mouse"><br><br>
 <input type="submit">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_submit_nn)

------

## Input Type Reset

`<input type="reset">`은 그들의 기본값으로 모든 폼 값들을 리셋시키는 버튼이다.

### 예제

```html
<form action="/action_page.php">
 First name:<br>
 <input type="text" name="firstname" value="Mickey"><br>
 Last name:<br>
 <input type="text" name="lastname" value="Mouse"><br><br>
 <input type="submit" value="Submit">
 <input type="reset">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_reset)

만약 네가 인풋값을 변화시키고 리셋버튼을 클릭하면 폼데이터는 다시 기본값으로 되돌릴 것이다.

------

## Input Type Radio

`<input type="radio">`는 라디오 버튼을 정의한다.

라디오 버튼은 유저에게 제한된 선택의 수 중에서 하나만을 고르게 한다.

### 예제

```html
<form>
 <input type="radio" name="gender" value="male" checked> Male<br>
 <input type="radio" name="gender" value="female"> Female<br>
 <input type="radio" name="gender" value="other"> Other
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_radio)

------

## Input Type Checkbox

`<input type="checkbox">`는 체크박스를 정의한다.

체크박스는 유저에게 0개 또는 더많은 옵션들을 선택할 수 있게한다.

### 예제

```html
<form>
 <input type="checkbox" name="vehicle1" value="Bike"> I have a bike<br>
 <input type="checkbox" name="vehicle2" value="Car"> I have a car
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_checkbox)

------

## Input Type Button

`<input type="button">` 은 버튼을 정의한다.

### 예제

```html
<input type="button" onclick="alert('Hello World!')" value="Click Me!">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_button)

------

## HTML5 Input Types

HTML5 에서는 새로운 인풋 타입들이 추가되었다.

- date
- datetime-local
- email
- month
- number
- range
- search
- tel
- time
- url
- week

새로운 인풋타입은 오래된 웹브라우저에서는 지원되지않는다. 이것들은 오래된곳에서는 `<input type="text">`로 동작할 것이다.

------

## Input Type Color

`<input type="color">`는 색깔이 포함된 인풋필드를 사용한다.

브라우저가 지원하면 색상 선택기가 인풋필드에 보여질 수 있다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 Select your favorite color:
 <input type="color" name="favcolor">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_color)

------

## Input Type Date

`<input type="date">`는 날짜가 포함된 인풋필드를 사용한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/incompatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 Birthday:
 <input type="date" name="bday">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_date)

너는 최소나 최대값 속성을 날짜에 제한하는것을 추가하기위해 사용할 수 있다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/incompatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 Enter a date before 1980-01-01:
 <input type="date" name="bday" max="1979-12-31"><br>
 Enter a date after 2000-01-01:
 <input type="date" name="bday" min="2000-01-02"><br>
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_date_max_min)

------

## Input Type Datetime-local

`<input type="datetime-local">`은 날짜와 시간인풋필드에 특화되어있다. 그리고 time zone이 없다. 브라우저가 지원하면 날짜 선택기를 인풋필드에 보여준다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/incompatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/incompatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 Birthday (date and time):
 <input type="datetime-local" name="bdaytime">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_datetime-local)

------

## Input Type Email

`<input type="email">`은 이메일 주소가 포함된 인풋필드이다.

브라우저가 지원하면 이메일 주소는 자동적으로 제출될 때 그것이 타당한지 체크해준다.

몇몇 스마트폰은 이메일 타입을 인식하고 .com을  이메일 인풋에 맞게 추가한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 E-mail:
 <input type="email" name="email">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_email)

------

## Input Type File

`<input type="file">`은 파일 선택 필드를 정의하고 파일을 업로드할 수 있는 버튼을 추가한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 Select a file: <input type="file" name="myFile">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_file)

------

## Input Type Month

`<input type="month">`는 유저에게 달과 년도를 선택하도록 한다.

브라우저가 지원하면 날짜 선택기를 인풋필드에 보여준다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/incompatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/incompatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 Birthday (month and year):
 <input type="month" name="bdaymonth">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_month)

------

## Input Type Number

`<input type="number">`는 수의 인풋필드를 정의한다.

너는 또한 받아들일 수있는 수를 제한할 수있다.

다음의 예는 숫자인풋필드를 보여주며 그것은 1에서부터 5까지 값이 들어올 수 있다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 Quantity (between 1 and 5):
 <input type="number" name="quantity" min="1" max="5">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_number)

------

## Input Restrictions

여기에 일반적인 공통 제한들이 있다.

| 속성      | 설명                                                         |
| :-------- | :----------------------------------------------------------- |
| checked   | 페이지가로드 될 때 입력 필드를 미리 선택하도록 지정합니다 (type = "checkbox"또는 type = "radio"의 경우). |
| disabled  | 입력 필드를 비활성화하도록 지정                              |
| max       | 입력 필드의 최대 값을 지정                                   |
| maxlength | 입력 필드의 최대 문자 수를 지정                              |
| min       | 입력 필드의 최소값을 지정                                    |
| pattern   | 입력 값을 확인할 정규식을 지정                               |
| readonly  | 입력 필드가 읽기 전용임을 지정 (변경 불가)                   |
| required  | 입력 필드가 필수임을 지정 (채워야 함).                       |
| size      | 입력 필드의 너비 (문자)를 지정                               |
| step      | 입력 필드의 유효한 숫자 간격을 지정                          |
| value     | 입력 필드의 기본값을 지정                                    |

너는 다음 챕터에서 인풋제한에 대하여 더 배울 수있다.

다음 예제는 숫자 인풋필드를 보여주며 이것은 값을 0에서 100까지 제한하고 10씩 건너뛰게 해준다. 또한 기본값은 30이다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 Quantity:
 <input type="number" name="points" min="0" max="100" step="10" value="30">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_number_step)

------

## Input Type Range

`<input type="range">`는 중요하지 않은 값의 수가 들어오는것을 통제한다. 기본값은 0에서부터 100이다. 그러나 너는 min, max, step 속성을 통해 받아들이는 값을 제한할 수 있다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 <input type="range" name="points" min="0" max="10">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_range)

------

## Input Type Search

`<input type="search">`는 탐색 필드에 사용된다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 Search Google:
 <input type="search" name="googlesearch">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_search)

------

## Input Type Tel

`<input type="tel">`은 전화번호가 포함된 인풋필드를 사용한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 Telephone:
 <input type="tel" name="phone" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_tel)

------

## Input Type Time

`<input type="time">`은 시간을 고를 수 있도록 해준다.

브라우가 지원하면 시간선택기를 인풋필드 안에 보여줄 수 있다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/incompatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 Select a time:
 <input type="time" name="usr_time">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_time)

------

## Input Type Url

`<input type="url">`은 URL 주소가 포함된 인풋필드를 사용한다.

브라우저가 지원하면 url 필드는 자동적으로 제출될 때 타당한지를 검사한다.

몇몇 스마트폰은 url 타입을 인식하여 url input을 맞게하기 위하여 키보드에 .com을 추가한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 Add your homepage:
 <input type="url" name="homepage">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_url)

------

## Input Type Week

`<input type="week">`는 유저에게 주와 년도를 선택할 수 있도록 한다.

브라우저가 지원하면 날짜 선택기를 인풋필드에 보여준다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/incompatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/incompatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form>
 Select a week:
 <input type="week" name="week_year">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_week)

------

## HTML Input Type Attribute

| 태그                                                         | 설명                        |
| :----------------------------------------------------------- | :-------------------------- |
| [`<input type="">`](https://www.w3schools.com/tags/att_input_type.asp) | 인풋의 속성을 결정하는 태그 |

[HTML Input Attributes](./HTML_inputattributes.md)