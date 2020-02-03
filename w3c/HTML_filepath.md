# HTML File Paths

------

| 경로                              | 설명                                                         |
| :-------------------------------- | :----------------------------------------------------------- |
| `<img src="picture.jpg">`         | picture.jpg는 현재페이지의 같은 폴더안에 위치해있다.         |
| `<img src="images/picture.jpg">`  | picture.jpg는 현재 폴더에 이미지 폴더안에 위치해있다.        |
| `<img src="/images/picture.jpg">` | picture.jpg는 현재 웹의 루트에서 이미지폴더에 위치해있다.    |
| `<img src="../picture.jpg">`      | picture.jpg는 현재 폴더로부터 하나의 수준위의 폴더에 위치해있다. |

------

## HTML File Paths

파일 경로는 웹사이트 폴더 구조안에 파일의 위치를 묘사한다.

파일 경로는 외부파일에 링크를 걸 때 사용한다.

- 웹페이지
- 이미지
- 스타일시트
- 자바스크립트

------

## Absolute File Paths

절대 파일 경로는 인터넷파일의 full URL이다.

### 예제

```html
<img src="https://www.w3schools.com/images/picture.jpg" alt="Mountain">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_files_absoulute)

`<img> `태그는 여기에 설명되어 있다 -->[HTML Images](https://www.w3schools.com/html/html_images.asp).

------

## Relative File Paths

상대 파일 경로는 현재 페이지에서 상대적인 파일 경로를 가리킨다.

이 예제에서 파일경로는 현재웹의 루트에 위치된 이미지폴더에 있는 파일을 가리킨다.

### 예제

```html
<img src="/images/picture.jpg" alt="Mountain">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_files_relative)

이 예제에서 파일 경로는 현재 폴더안에 이미지 폴더에 있는 파일을 가리킨다.

### 예제

```html
<img src="images/picture.jpg" alt="Mountain">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_files_relative_1)

이 예제에서 파일 경로는 현재 폴더 위의 수준에 폴더에 위치되어 있는 이미지 폴더를 가리킨다.

### 예제

```html
<img src="../images/picture.jpg" alt="Mountain">
```

[Try it Yourself »](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_files_relative_2)

------

## Best Practice

이것은 상대 파일경로를 사용하는 것이 가장 좋은 연습이다.

상대 파일 경로를 사용할 때, 너의 웹 페이지는 현재 base URL에 bound되지 않을 것이다. 모든 링크들은 너의 컴퓨터에서 너의 현재 도메인뿐만 아니라 미래의 도메인 에서도 잘 돌아가게 될 것이다.

[HTML Head](./HTML_head.md)

