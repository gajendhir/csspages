<image src='./images/cssflex.svg' width='100%'/>

[Home](./readme.md) 

[<img src='./dslogo.png' align='left' width='100' alt='logo'/>](http://www.dataspec.info)

# FlexBox Layout in CSS

The **FlexBox layout** is initiated with the `display: flex;` property and effects the way the children of the element are laid-out on the webpage.

```css
(CSS)
.parent {
	display: flex;
	... other properties
}
```

```html
(HTML)
<div class='parent'>
	<div class='child1'>
		...content of child 1
	</div>
	<div class='child2'>
		...content of child 2
	</div>
	....
</div>
```

Each item laid-out inside a flexbox is called *flex item*. The flexbox itself is referred to as the *flex container*. 

The layout of flex items can be in either horizontal or vertical direction.


## Main and Cross Axes

The direction in the items are laid out is known as the *main axis* and the direction perpendicular to the main axis is known as the *cross axis*. 

`row` is the main axis by default.

Default `width` is `100%` when main axis is row, and when the main axis is column the default `height` is the height required to render the content.

The size of a flex item along the main axis is identified as the *main size*, where as its size along the cross axis is the  *cross size*

## properties for the flexbox

Flexbox has some properties applicable at the parent and child levels that can be used to create innovative layouts. 

### At parent (or container) level...

* `justify-content`

	Justifies the overall content along the **main axis**.

* `justify-items` <a id='justifyitems'></a>

	Justifies the individual elements along the main axis within the dimensions designated to it after `justify-content` is processed.

	This setting applies to each of the elements in the flexbox, unless a `justify-self` is specified to an element at the child level.

* `align-content`

	Aligns the overall content along the **cross axis**.

* `align-items` <a id='alignitems'></a>

	Aligns the indiviual elements along the cross axis within the dimensions designated to it after `align-content` is processed.

	This alignment is applied to each of element in the flexbox, unless a `align-self` is specified at the child level.

* `place-content`

	This is a shorthand property for 
	* `align-content`, and 
	* `justify-content`.

	If one value is provided, that value applied to both `align-content` and `justify-content`. 

	If two values are provided, the first will be for `align-content` and the second will be for `justify-content`.

* `place-items` <a id='placeitems'></a>

	This is a shorthand property for 
	* `align-items` and
	* `justify-items`.

	If one value is provided, that value applied to both `align-items` and `justify-items`. 
	
	If two values are provided, the first will be for `align-items` and the second will be for `justify-items`.

* `flex-direction`

	determins the direction in which items are placed in the flex container.

	When the direction is `row` or `row-reverse` the main axis is in the horizontal direction.

	![flex-row](./images/flex-row.svg)

	Similarly, when the direction is `column` or `column-reverse` the main axis is in the vertical direction.

	![flex-column](./images/flex-column.svg)

* `flex-wrap`

	determins whether are items are forced in one line or may wrap onto multiple lines.

* `flex-flow`

	This is the shorthand property for...
	* `flex-direction`
	* `flex-wrap`

* `column-gap`

	Determines the gap between columns in the `flex` box. Also works for `grid` and `multi-column` container.

* `row-gap`

	Determines the gap between rows in the `flex` and `grid` containers

* `gap`

	This is the shorthand property for...
	* `column-gap`
	* `row-gap`

### At child level...

* `flex`

	This is shorthand property for...
	* [`flex-grow`](#flexgrow)
	* [`flex-shrink`](#flexshrink)
	* [`flex-basis`](#flexshrink)
	
* `flex-grow` <a id='flexgrow'></a>

	This determines how the *positive free space* in the flex container is assigned to the *main-size* of the item i.e. it specifies the grow factor for an item.

* `flex-shrink` <a id='flexshrink'></a>

	This determines how the *negative free space* in the flex container is assigned to the *main-size* of the item i.e. it specifies the shrink factor for an item.

* `flex-basis` <a id='flexbasis'></a>

	This specifies the initial main size for the flex item. The final computed main size will depend on the `flex-grow` and `flex-shrink` values.

* `order`

	The `order` property defines the sequence in which each flex item is rendered.

* `align-self`

	This property overrides the [`align-items`](#alignitems) property defined for the flex container.

* `justify-self`

	This property overrides the [`justify-items`](#justifyitems) property defined for the flex container.

* `place-self`

	This property overrides the [`place-items`](#placeitems) property defined for the flex container.

<<<<<<< HEAD
=======

>>>>>>> 6b7afbc45804e6be53ff9663ecce5cd6f920896e

[Home](./readme.md) 
