# Size of a Box in CSS

The layout of elements on the document is done as rectangular boxes, based on the CSS Box Model. 

An understanding of the the Box Model goes a long way in achieving the desired UI/UX.

## Areas and Boxes

A box has 4 areas or parts...

### content-area

This is the area where the actual content - text, images or other HTML elements - area displayed. 
	
### padding-area

specified as `padding` or using the `padding-*` sub-properties.

This is the area surrounds the content-area and extends to the outer edge of the padding on each side.

### border-area

specified as `border` or using the `border-*` sub-properties.

The area surrounding the padding-area and extending up to the edge of the border size on each side.

### margin-area

specified as `margin` or using the `margin-*` sub-properties.

The area surrounding the border-area and extending up to the edge of the margin specified on each side.

## The Box

The areas bring us to the different boxes used by each element... 

- **content-box** - it is the innermost box of the element that renders the content area with the actual content - text, images and other elements.

- **padding-box** - the outer edge of the padding area. If padding is 0, then padding-box will be same as content-box. 

- **border-box** - starts from the outer area of the padding-box up to the outer edge of the border-area. 

- **margin-box** - the area of the element up to the outer edge of the margin-area.

- **visual-box** - the box that is seen on the web page, this includes the content, padding and border. The margin is not a part of this. 

- **layout-box** - the space occupied by the element on the document - including its content, padding, border and margin. This value is used for layout and position on the document.

- **paint-box** - this is the paintable area of the element. This area is the excludes the _margin-area_.

- **coord-box** - this is the location and size of the element within its parent. These coordinates exclude the margin area (of the parent).

## `box-sizing`

CSS allows for two box-sizing computations.

### `content-box`

```css
	.box {
		box-sizing: content-box;
		...
	}
```

In a `content-box`, the `width` and `height` properties specified denote the dimension of the content-area. The padding, border etc add on to this to compute the `<layout-box>`.

### `border-box`

```css
	.box {
		box-sizing: border-box;
		...
	}
```

In a `border-box`, the `width` and `height` properties specified set the dimensions of the `<paint-box>`, i.e. the padding and border areas are include within the `width` and `height`.



