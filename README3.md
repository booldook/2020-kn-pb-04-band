# 가운데 정렬, Float
## 가운데 정렬
### 인라인요소 정렬 
- text-align을 포함한 모든 **글자와 관련**된 속성은 상속이 된다.
1. text-align
2. font-size
3. color
4. line-height ...

### 블럭요소 정렬
- div, p, h 등 layout(block, box)요소들은 자기가 가운데로 가야한다.

```css
.box {margin: 0 auto;}
```

## Float(중요!!!!)
- float는 태그를 inline속성으로 바꿔준다.
- inline요소와 float요소가 만나면 어울려진다.
- 사이트 레이아웃을 잡을때 많이 사용된다.

```html
<div class="header">
	<div class="lt">Left</div>
	<div class="rt">Right</div>
	<div class="clearfix"></div>
</div>
```

```css
.lt {float: left;}	/* 띄워서 왼쪽에 가져다 놓는다 */
.rt {float: right;}	/* 띄워서 오른쪽에 가져다 놓는다 */
.clearfix {clear: both;} /* 내 부모 안에서 내 위에 있는 모든 float요소를 가라앉힌다. */
```

## 이미지를 반응형으로 만들기
- 이미지에 width, height를 주지 않고 사용하면 이미지 본래의 크기로 표현된다.
- 반응형으로 이미지를 사용하기 위해서는 이미지 감싸고 있는 부모의 사이즈에 맞춰서 **%**로 표현한다. 
```css
.img {width: 100%;}
.img {width: 100%; max-width: 1000px;}
```

## box-sizing
- block 요소의 사이즈를 측정할 때 css는 기본값(box-sizing: content-box)이 내용의 크기로 지정되므로, 작업하는데 불편하다. 그래서 아래와 같이 block요소들의 사이즈 값의 측정방법을 바꾼다.

```css
h1, h2, h3, h4, h5, h6, div, p {box-sizing: border-box;}
```