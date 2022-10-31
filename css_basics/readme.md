## box model

- content area
- padding area(內距)
- border area(邊框)
- margin area(外距)
    - margin: 0 auto → 水平居中
- 元素所佔用的視覺空間 = content + padding + border

### Box-sizing

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

### 1. em

以closest parent為標準計算尺寸

1 `em`= 16 `px`

### 2. rem

以html為標準計算尺寸

### 3. Percentage

以closest parent為標準計算尺寸

### 4. vh/vw

viewport長度的比例

## [Position](https://dev.to/jenhsuan/day-31-of-100daysofcode-review-css-position-4ba5)
### 1. Static
static is the default position style. The static components will be placed from left and top corner of the viewport.

### 2. Relative
The relative components have the following properties:

1. The component will be moved relative to the original position(static) according to top, left, right
2. Moved component will not affect other components.
3. The original position(static) will still be available.

### 3. Absolute
The absolute components depends on the position style of the parent component. There are two conditions.

1. Condition 1: if the position style of the parent component is default (static)
* It will perform as fixed

2. Condition 2: if the position style of the parent component is one of the following position style.
* relative | absolute | fixed | inherit
* The absolute component will move with the parent component when scrolling the window

### 4. Fixed
Scroll the window from the following CodePen example. The fixed components have the following properties:

1. The fixed component is fixed to the viewport even we scroll the window.
2. The width of the fixed component changes (no longer as long as the mother box)
3. The original position(static) will be unavailable.

### 5. Sticky
The sticky component performs as a relative component before it arrives the position we set top, left, right

## Overflow
* visible
* hidden
* auto
* scroll