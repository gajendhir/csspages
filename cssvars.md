# Variables or Custom Properties in CSS

## Declare 

### use -- (2 dashes)

Specify, two dashes followed by a name for the custom property and assign a valid CSS value.

```CSS

:root {
    --my-forecolor: red;
}

```


### use @property

```CSS

@property --my-forecolor {
    syntax: <color>;
    inherits: false;
    initial-value: darkblue;
}

```

## Use a Custom Property

The value in the custom variable can be referenced by using it with a var().

```CSS

.heading {
    color: var(--my-forecolor);
}

```

