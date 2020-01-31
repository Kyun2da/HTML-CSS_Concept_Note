# HTML Images

이미지는 웹페이지의 모습과 디자인을 향상시킬 수 있다.

### 예제

```html
<img src="pic_trulli.jpg" alt="Italian Trulli">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_trulli)

### 예제

```html
<img src="img_girl.jpg" alt="Girl in a jacket">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_girl)

### 예제

```html
<img src="img_chania.jpg" alt="Flowers in Chania">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_chania)

------

## HTML Images Syntax

HTML에서 이미지는 `<img>`태그로 정의된다.

`<img>`태그는 비어있으며 그것은 오직 속성만을 포함하고 닫는태그 또한 필요하지 않다.

`src`속성은 이미지의 URL을 넣는 곳이다.

```html
<img src="url">
```



------

## The alt Attribute

alt속성은 만약 사용자가 어떠한 이유로 이미지를 볼 수 없다면  이미지를 텍스트로 대체하기위해 공급되는 속성이다. 

이미지의 `alt`속성은 이미지를 묘사해야만 한다.

### 예제

```html
<img src="img_chania.jpg" alt="Flowers in Chania">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_alt_chania)

만약 브라우저가 이미지를 찾을 수 없다면 그것은 `alt`속성을 보여준다

### 예제

```html
<img src="wrongname.gif" alt="Flowers in Chania">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_wrongname)

**Note:** `alt`속성은 웹페이지의 유효성검사 때문에라도 필요하다.



## Image Size - Width and Height

너는 `style`속성을 이미지의 높이나 넓이를 조절하기위해 사용할  수 있다.

### 예제

```html
<img src="img_girl.jpg" alt="Girl in a jacket" style="width:500px;height:600px;">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_size)

대안으로 너는 넓이와 높이 속성또한 사용할 수 있다.

### 예제

```html
<img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_attributes)

넓이와 높이 속성은 항상 픽셀로 이미지의 넓이와 높이를 정의한다.

**Note:** 항상 이미지의 높이와 넓이를 정의해라 만약 넓이와 높이가 정의되어 있지 않는다면 페이지는 아마도 이미지를 로딩하는 동안 페이지가 깜박거릴 수 있다.

------

## Width and Height, or Style?

넓이와 높이 그리고 스타일 속성은 HTML에서 유효하다.

그러나 우리가 스타일 속성을 사용한다면 그것은 스타일시트가 이미지의 사이즈를 바꾸는  것을 막을 것이다.

### 예제

```html
<!DOCTYPE html>
<html>
<head>
<style>
img {
 width: 100%;
}
</style>
</head>
<body>

<img src="html5.gif" alt="HTML5 Icon" width="128" height="128">
<img src="html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">

</body>
</html>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_style)

------

## Images in Another Folder

만약 경로를 지정하지 않으면 브라우저는 같은 폴더에서 경로를 찾을 것이다.

하지만 하나의 서브폴더에 이미지를 저장하는 것이 일반적이며 너는 반드시 `src`속성에 그 폴더 이름을 포함해야만 한다.

### 예제

```html
<img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_folder)

------

## Images on Another Server

몇몇 웹사이트들은 그들의 이미지를 이미지 서버에 저장한다.

실제로 너는 세상의 어떤 웹사이트에서든지 이미지에 접근할 수 있다.

### 예제

```html
<img src="https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_w3schools)

더 읽고싶다면 오른쪽의 파일 경로 페이지를 참조하라 [HTML File Paths](https://www.w3schools.com/html/html_filepaths.asp).

------

## Animated Images

 HTML은 GIF를 허용한다.

### 예제

```html
<img src="programming.gif" alt="Computer Man" style="width:48px;height:48px;">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_hackman)

------

## Image as a Link

`a`태그안에 `img`태그를 넣어서 이미지를 링크로서 활용할 수 있다.

### 예제

```html
<a href="default.asp">  <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;border:0;"></a>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_link)

**Note:** `border:0;`은 IE9가 이미지의 테두리를 표시하는것을 방지하기위해 넣어두었다.

------

## Image Floating

CSS `float`속성은 이미지가 텍스트의 왼쪽이나 오른쪽에 있을 수 있도록 허락한다.

### 예제

```php+HTML
<p><img src="smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">The image will float to the right of the text.</p>
<p><img src="smiley.gif" alt="Smiley face" style="float:left;width:42px;height:42px;">The image will float to the left of the text.</p>
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_float)

**Tip:** CSS Float에 대해 공부하고 싶다면 이곳을 참조해라 [CSS Float Tutorial](https://www.w3schools.com/css/css_float.asp).

------

## HTML Screen Readers

스크린 리더는 HTML 코드를 읽어주는 소프트웨어 프로그램이다. 이것은 텍스트를 변환하고 유저가 이 내용을 들을 수 있도록 해준다. 스크린 리더는 시각 장애인들이나 학습장애인들에 게 유용하다.

------

## Chapter Summary

- `<img>` 태그를 이미지를 정의할 때 사용하라
- `src`속성을 image의 URL을 정의할 때 사용해라
- `alt`속성을 이미지의 대체텍스트를 정의할 때 사용해라 이것은 표시되지 않을 수 있다.
- HTML `width`와 `height`속성을 이미지의 크기를 정의할 때 사용하라
- CSS `width`와 `height`속성은 이미지의 사이지를정의할 때 대안적으로 사용해라
- `float`속성을 이미지의 float를 허락할 때 사용하라



------

## HTML Image Tags

| 태그        | 설명                                             |
| :---------- | :----------------------------------------------- |
| `<img>`     | 이미지를 정의한다.                               |
| `<map>`     | 이미지 맵을 정의한다.                            |
| `<area>`    | 이미지맵안에 클릭할 수 있는 영역을 정의한다.     |
| `<picture>` | 다수의 이미지 리소스를 위한 컨테이너를 정의한다. |

[HTML Tables](./HTML_tables.md)