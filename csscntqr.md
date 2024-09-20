# Container Queries in CSS

## Register a Container

Register an element as a `container`.

```CSS
.parent {
    container-name: myname;
    container-type: inline-size;
}
```

or, use the shorthand option

```CSS
container: myname / inline-size;
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

style-feature

* `style(property: value)`

`property` to be checked for `value`.