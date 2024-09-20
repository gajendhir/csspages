# flex Layout in CSS

The flex layout is initiated with the `display: flex;` property and effects the children of the element having this property.

```CSS
(CSS)
.parent {
	display: flex;
	... other properties
}
```

```HTML
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

## properties of the flex group

At parent level...

* justify-content
* align-items
* place-items
* flex-direction
* flex-wrap

At child level...

* flex
* flex-basis
* flex-shrink
* flex-grow
* align-self
* order