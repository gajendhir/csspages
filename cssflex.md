[Home](./readme.md) 

# FlexBox Layout in CSS

The **FlexBox layout** is initiated with the `display: flex;` property and effects the children of the element having this property.

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

## Main and Cross Axes

>The main and cross axes for flexbox is decided by the `flow-direction` property.

`row` is the main axis by default.


Default `width` is `100%` when main axis is row, and when the main axis is column the default `height` is the height required to render the content.





## properties for the flexbox group

Flexbox has some properties applicable at the parent and child levels that can be used to create innovative layouts. 

### At parent (or container) element...

* `justify-content`
* `align-items`
* `place-items`
* `flex-direction`
* `flex-wrap`
* `gap`
* `row-gap`
* `column-gap`

### At child elements...

* `flex`
* `flex-grow`
* `flex-shrink`
* `flex-basis`
* `order`
* `align-self`
* `justify-self`
* `place-self`


[Home](./readme.md) 
