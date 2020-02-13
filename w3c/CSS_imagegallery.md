# CSS Image Gallery

CSS 는 이미지 갤러리를 만들 수 있다.

------

## Image Gallery

### 예제

```html
<html>
<head>
<style>
div.gallery {
  margin: 5px;
  border: 1px solid #ccc;
  float: left;
  width: 180px;
}

div.gallery:hover {
  border: 1px solid #777;
}

div.gallery img {
  width: 100%;
  height: auto;
}

div.desc {
  padding: 15px;
  text-align: center;
}
</style>
</head>
<body>

<div class="gallery">
  <a target="_blank" href="img_5terre.jpg">
    <img src="img_5terre.jpg" alt="Cinque Terre" width="600" height="400">
  </a>
  <div class="desc">Add a description of the image here</div>
</div>

<div class="gallery">
  <a target="_blank" href="img_forest.jpg">
    <img src="img_forest.jpg" alt="Forest" width="600" height="400">
  </a>
  <div class="desc">Add a description of the image here</div>
</div>

<div class="gallery">
  <a target="_blank" href="img_lights.jpg">
    <img src="img_lights.jpg" alt="Northern Lights" width="600" height="400">
  </a>
  <div class="desc">Add a description of the image here</div>
</div>

<div class="gallery">
  <a target="_blank" href="img_mountains.jpg">
    <img src="img_mountains.jpg" alt="Mountains" width="600" height="400">
  </a>
  <div class="desc">Add a description of the image here</div>
</div>

</body>
</html>
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_image_gallery)

------

## 더 많은 예제

### Responsive Image Gallery

CSS 미디어 쿼리를 사용하여 데스크톱, 태블릿 및 스마트 폰에서 잘 보이는 반응 형 이미지 갤러리를 만드는 방법

![img](https://www.w3schools.com/css/responsiveImgGallery.jpg)

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_image_gallery_responsive)

[CSS Image Sprites](./CSS_imagesprites.md)