# Container Queries in CSS

## Register a Container

Register an element as a `container`.

```CSS

.parent {
    container-name: myname;
    container-type: inline-size;
    ... other code
}

```

or, use the shorthand option

```CSS

.parent {
    container: myname / inline-size;
    ... other code
}

```

## Query a Container

```CSS

div {
    font-size: 2em;
}

@container myname (width: > 30ch)
{
    div {
        font-size: 3em;
    }
}

```
## CSS Properties for Containers

### Container Type

container-type: ...

* `size`
* `inline-size`
* `normal`

### Container Name

container-name: ...

### Container Condition

size-query supports...

* `width`
* `height`
* `inline-size`
* `block-size`
* `aspect-ratio`
* `orientation`

style-query

* `style(property: value)`

`property` to be checked for `value`.