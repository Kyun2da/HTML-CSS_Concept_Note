# CSS Combinators

## CSS Combinators

Combinator는 선택기 간의 관계를 설명하는 것이다.

CSS 선택기는 둘 이상의 간단한 선택기를 포함 할 수 있다. 간단한 선택기 사이에 결합기를 포함시킬 수 있다.

CSS에는 4 가지 조합이 있다 :

- 자손선택자 (space)
- 자식 선택자 (>)
- 인접한 형제 선택자 (+)
- 일반 형제 선택자 (~)

------

## Descendant Selector

자손 선택기는 지정된 요소의 자손 인 모든 요소와 일치한다.

다음 예제는 `<div>` 요소 내의 모든 `<p>` 요소를 선택한다.

### 예제

```css
div p {
 background-color: yellow;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_sel_element_element)

------

## Child Selector

자식 선택기는 지정된 요소의 자식 인 모든 요소를 선택한다.

다음 예제는 `<div>` 요소의 하위 요소 인 모든 `<p>` 요소를 선택한다.

### 예제

```css
div > p {
 background-color: yellow;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_sel_element_gt) <- 이곳 들어가면 Descendant와 Child의 차이가 뭔지 이해가 감

------

<iframe id="google_ads_iframe_/22152718/sws-hb//w3schools.com//mid_content_0" title="3rd party ad content" name="google_ads_iframe_/22152718/sws-hb//w3schools.com//mid_content_0" width="728" height="90" scrolling="no" marginwidth="0" marginheight="0" frameborder="0" srcdoc="" data-google-container-id="4" data-load-complete="true" style="box-sizing: inherit; border: 0px; vertical-align: bottom;"></iframe>

------

## Adjacent Sibling Selector

인접 형제 선택기는 지정된 요소의 인접 형제 인 모든 요소를 선택한다.

형제 요소는 동일한 부모 요소를 가져야하며 "인접한"은 "즉시 다음"을 의미한다.

다음 예제는 `<div>` 요소 바로 뒤에 배치 된 모든 `<p> ` 요소를 선택한다.

### 예제

```css
div + p {
 background-color: yellow;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_sel_element_pluss)

------

## General Sibling Selector

일반 형제 선택기는 지정된 요소의 형제 인 모든 요소를 선택한다.

다음 예제는 `<div>` 요소의 형제 인 모든 `<p>` 요소를 선택한다.

### 예제

```css
div ~ p {
 background-color: yellow;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_sel_element_tilde)

------

## All CSS Combinator Selectors

| 선택자                                                       | 예제    | 설명                                                   |
| :----------------------------------------------------------- | :------ | :----------------------------------------------------- |
| [*element* *element*](https://www.w3schools.com/cssref/sel_element_element.asp) | div p   | <div> 요소 내의 모든 <p> 요소를 선택한다               |
| [*element*>*element*](https://www.w3schools.com/cssref/sel_element_gt.asp) | div > p | 부모가 <div> 요소 인 모든 <p> 요소를 선택한다.         |
| [*element*+*element*](https://www.w3schools.com/cssref/sel_element_pluss.asp) | div + p | <div> 요소 바로 뒤에 배치 된 모든 <p> 요소를 선택한다. |
| [*element1*~*element2*](https://www.w3schools.com/cssref/sel_gen_sibling.asp) | p ~ ul  | <p> 요소가 앞에 오는 모든 <ul> 요소를 선택한다         |

[CSS Pseudo-class](./CSS_pseudoclasses.md)