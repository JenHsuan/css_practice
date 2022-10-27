## box model

- content area
- padding area(內距)
- border area(邊框)
- margin area(外距)
    - margin: 0 auto → 水平居中
- 元素所佔用的視覺空間 = content + padding + border

### box-sizing:

計算長寬的方式

```css
1. box-sizing: content-box
```

- content width = width
- content height = height

```css
2. box-sizing: border-box 
```

- content width = width - border-width - padding-width
- content width = width - border-width - padding-width
- 讓padding與border不會增加視覺空間的寬度

## Pseudo classes

Define special state of an element

```css
a:hover
```

## Pseudo elements

Define style for special part of an element

```css
h1::hover
```

## Measurement

### em

以parent為標準計算尺寸

1 `em`= 16 `px`

### rem

以html為標準計算尺寸
