<image src='./csscntqy.png' width='100%'/>

[Home](./readme.md) 

# Container Queries in CSS

First a container must be registered, and it can be queried. 

## Register a Container

Use a selector to register a `container`.

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

At the time of registration, two details - `type` and `name` - have to specified.

### Container Type

`container-type: ...`

* `size`
* `inline-size`
* `normal`

### Container Name

`container-name: <nameofcontainer>;`

`<nameofcontainer>` identifies the container especially useful if you may a scenario of multiple containers.

## Query a Container

The container query starts with the `@container` at-rule followed by the name of the container and the feature query.

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
container query to set `font-size` for the `div` inside the `myname` container to `3em` if the feature `width` is greater than `30ch`.

### Query Conditions

size-query...

* `width`
* `height`
* `inline-size`
* `block-size`
* `aspect-ratio`
* `orientation`

style-query...

* `style(property: value)`

`property` to be checked for `value`.

for eg
```css
@container contname style('background-color: blue') {
    ... 
    styles 
    ...
}
```
The container query to apply styles if the `background-color` of the container `contname` is blue 

### Compound Queries

`and`, `or` and `not` can be used to create compound queries

for eg
```css
    @container myname (width>30ch) and (height>100px) {
        ...
    }

    @container myname not (color: blue) {
        ...
    }
```

### Nested Container Queries

Container queries can be nested within other container queries.

for eg
```css
    @container myname (width>30ch) {
        ...
        @container myname not (background-color: blue) {
            ...
        }
        @container myname not (background-color: red) {
            ...
        }
    }
```


[Home](./readme.md)