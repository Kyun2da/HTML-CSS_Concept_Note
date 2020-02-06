# HTML Form Elements

이 챕터는 모든 HTML 폼 엘리먼트에 대해 묘사합니다.

------

## The `<input>` Element

가장 중요한 폼 엘리먼트는 `<input>`엘리먼트이다.

이 `<input>`엘리먼트는 각각의 방식으로 보여 질 수 있고 `type`속성에 의존한다.

### 예제

```html
<input name="firstname" type="text">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_elem_input)

만약 type 속성이 생략된다면 인풋 필드는 기본속성인 text를 얻는다.

------

## The `<select>` Element

`<select>`엘리먼트는 드롭 다운 리스트를 정의한다.

### 예제

```html
<select name="cars">
 <option value="volvo">Volvo</option>
 <option value="saab">Saab</option>
 <option value="fiat">Fiat</option>
 <option value="audi">Audi</option>
</select>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_elem_select)

`<option>`엘리먼트는 선택될 수 있는 옵션을 정의한다.

기본값으로 첫번째 아이템이 드롭다운 리스트에 선택되어 있다.

미리 선택된 옵션을 정의하기 위해서 옵션에 `selected`속성을 추가하면된다.

### 예제

```html
<option value="fiat" selected>Fiat</option>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_elem_select_pre)

### 볼 수 있는 값 : 

`size`속성을 사용하면 볼 수 있는 값의 수를 특화시킬 수 있다.

### 예제

```html
<select name="cars" **size="3"**>
 <option value="volvo">Volvo</option>
 <option value="saab">Saab</option>
 <option value="fiat">Fiat</option>
 <option value="audi">Audi</option>
</select>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_elem_select_size)

### 다중 선택을 허용하기

`multiple`속성을 사용해서 하나의 값보다 더 많은 값을 선택할 수 있다.

### 예제

```html
<select name="cars" size="4" **multiple**>
 <option value="volvo">Volvo</option>
 <option value="saab">Saab</option>
 <option value="fiat">Fiat</option>
 <option value="audi">Audi</option>
</select>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_elem_select_multiple)

------

## The `<textarea>` Element

`<textarea>`엘리먼트는 인풋 필드의 다중라인을 정의한다.

### 예제

```html
<textarea name="message" rows="10" cols="30">
The cat was playing in the garden.
</textarea>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_elem_textarea)

너는 또한 CSS를 사용하여 텍스트구역의 크기를 정할 수 있다.

### 예제

```html
<textarea name="message" style="width:200px; height:600px;">
The cat was playing in the garden.
</textarea>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_elem_textarea_style)

## The `<button>` Element

`<button>`엘리먼트를 사용하여 클릭가능한 버튼을 만들 수 있다.

### 예제

```html
<button type="button" onclick="alert('Hello World!')">Click Me!</button>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_elem_button)

**Note:** 버튼 요소의 유형 속성을 항상 지정해라. 브라우저마다 버튼 요소에 다른 기본 유형을 사용할 수 있다.

------

## HTML5 폼 엘리먼트

HTML5 는 폼 엘리먼트 원소를 추가했다.

- `<datalist>`
- `<output>`

**Note:** 브라우저는 알려지지않은 엘리먼트를 보여주지 않는다. 오래된 브라우저에서 지원되지않는 새로운 엘리먼트들은 너의 웹페이지를 "파괴"하지는 않을 것이다.

------

## HTML5 `<datalist>` Element

`<datalist>` 요소는 `<input>` 요소에 대해 사전 정의 된 옵션 목록을 지정한다. 사용자는 데이터를 입력 할 때 사전 정의 된 옵션의 드롭 다운 목록을 볼 수 있다. `<input>` 요소의 list 속성은 `<datalist>` 요소의 id 속성을 참조해야한다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

```html
<form action="/action_page.php">
 <input list="browsers">
 <datalist id="browsers">
  <option value="Internet Explorer">
  <option value="Firefox">
  <option value="Chrome">
  <option value="Opera">
  <option value="Safari">
 </datalist>
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_elem_datalist)

------

## HTML5 `<output>` Element

`<output>`엘리먼트는 계산의 결과를 보여주는 엘리먼트이다.

![Opera](https://www.w3schools.com/images/compatible_opera2020.gif)![Safari](https://www.w3schools.com/images/compatible_safari2020.gif)![Chrome](https://www.w3schools.com/images/compatible_chrome2020.gif)![Firefox](https://www.w3schools.com/images/compatible_firefox2020.gif)![Internet Explorer](https://www.w3schools.com/images/compatible_edge2020.gif)

### 예제

`<output>`엘리먼트에서 계산을 수행해서 결과를 보여준다.

```html
<form action="/action_page.php"
 oninput="x.value=parseInt(a.value)+parseInt(b.value)">
 0
 <input type="range" id="a" name="a" value="50">
 100 +
 <input type="number" id="b" name="b" value="50">
 =
 <output name="x" for="a b"></output>
 <br><br>
 <input type="submit">
</form>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_elem_output)

------

## HTML Form Elements

| 태그                                                         | 설명                                             |
| :----------------------------------------------------------- | :----------------------------------------------- |
| [`<form>`](https://www.w3schools.com/tags/tag_form.asp)      | 사용자 입력을위한 HTML 양식을 정의               |
| [`<input>`](https://www.w3schools.com/tags/tag_input.asp)    | 입력 컨트롤을 정의                               |
| [`<textarea>`](https://www.w3schools.com/tags/tag_textarea.asp) | 여러 줄 입력 컨트롤 (텍스트 영역)을 정의         |
| [`<label>`](https://www.w3schools.com/tags/tag_label.asp)    | `<input>` 요소의 레이블을 정의                   |
| [`<fieldset>`](https://www.w3schools.com/tags/tag_fieldset.asp) | 관련 요소를 양식으로 그룹화                      |
| [`<legend>`](https://www.w3schools.com/tags/tag_legend.asp)  | `<fieldset>` 요소의 캡션을 정의                  |
| [`<select>`](https://www.w3schools.com/tags/tag_select.asp)  | 드롭 다운리스트를 정의                           |
| [`<optgroup>`](https://www.w3schools.com/tags/tag_optgroup.asp) | 드롭 다운 목록에서 관련 옵션 그룹을 정의         |
| [`<option>`](https://www.w3schools.com/tags/tag_option.asp)  | 드롭 다운 목록에서 옵션을 정의                   |
| [`<button>`](https://www.w3schools.com/tags/tag_button.asp)  | 클릭 가능한 버튼을 정의                          |
| [`<datalist>`](https://www.w3schools.com/tags/tag_datalist.asp) | 입력 컨트롤에 대해 미리 정의 된 옵션 목록을 지정 |
| [`<output>`](https://www.w3schools.com/tags/tag_output.asp)  | 계산 결과를 정의                                 |

[HTML Input Types](./HTML_inputtypes.md)