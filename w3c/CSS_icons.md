# CSS Icons

## 어떻게 아이콘을 추가하는가

너의 HTML 페이지에 아이콘을 추가하는 가장 간단한 방법은 Font Awesome과 같은 아이콘 라이브러리를 쓰는 것이다.

HTML 엘리먼트의 어떤 곳에서나 아이콘 클래스의 이름을 추가할 수있다. (`<i>`혹은 `<span>`)

모든 아이콘 라이브러리 아래에 있는 아이콘들은 스칼라화할 수 있는 벡터화 되어있으며 CSS로 커스터마이징이 가능하다(사이즈,색,그림자 등등)

------

## Font Awesome Icons

Font Awesome아이콘을 사용하기 위해서 [fontawesome.com](https://fontawesome.com/)으로 가서  로그인을 하고 `<head>`섹션에 넣을 수있는 코드를 얻으면 된다.

```html
<script src="https://kit.fontawesome.com/yourcode.js"></script>
```

Font Awesome에 대해 더 알고 싶다면 Font Awesome 튜토리얼을 참고하라 -> [Font Awesome 5 tutorial](https://www.w3schools.com/icons/fontawesome5_intro.asp).

**Note:** 다운로드나 설치가 필요없다!

### Example

```html
<!DOCTYPE html>
<html>
    <head>
        <script src="https://kit.fontawesome.com/a076d05399.js"></script>
    </head>
    <body>
        <i class="fas fa-cloud"></i>
        <i class="fas fa-heart"></i>
        <i class="fas fa-car"></i>
        <i class="fas fa-file"></i>
        <i class="fas fa-bars"></i>
    </body>
</html>
```

[Try It Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_icons_fa)

For a complete reference of all Font Awesome icons, visit our [Icon Reference](https://www.w3schools.com/icons/icons_reference.asp).

## Bootstrap Icons

부트스트랩 glyphicon들을 사용하기 위해서는 너의 HTML 페이지에 `<head>`섹션 안에 다음과 같은 라인을 추가해야 한다.

```html
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
```

**Note:** 다운로드나 설치가 필요가 없다!

### 예제

```html
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
</head>
<body>

<i class="glyphicon glyphicon-cloud"></i>
<i class="glyphicon glyphicon-remove"></i>
<i class="glyphicon glyphicon-user"></i>
<i class="glyphicon glyphicon-envelope"></i>
<i class="glyphicon glyphicon-thumbs-up"></i>

</body>
</html>
```

[Try It Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_icons_bs)

------

## Google Icons

구글 아이콘을 사용하기 위해서는 HTML페이지에 너의 `<head>`섹션에 다음과 같은 라인을 추가하면 된다.

```html
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
```

**Note:** 다운로드나 설치가 필요가 없다.

### 예제

```html
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
</head>
<body>

<i class="material-icons">cloud</i>
<i class="material-icons">favorite</i>
<i class="material-icons">attachment</i>
<i class="material-icons">computer</i>
<i class="material-icons">traffic</i>

</body>
</html>
```

[Try It Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_icons_google)

완전한 아이콘들에 대해 알고싶다면 이 아이콘 튜토리얼을 가보아라 [Icon Tutorial](https://www.w3schools.com/icons/default.asp).



[CSS Links](./CSS_links.md)

