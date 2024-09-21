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

## properties for the flexbox group

Flexbox has some properties applicable at the parent and child levels that can be used to create innovative layouts. 

### At parent (or container) element...

* `justify-content`
* `align-items`
* `place-items`
* `flex-direction`
* `flex-wrap`
* `gap`, `row-gap`, `column-gap`

### At child elements...

* `flex`
* `flex-basis`
* `flex-shrink`
* `flex-grow`
* `order`
* `align-self`
* `justify-self`
* `place-self`


[Home](./readme.md) 
