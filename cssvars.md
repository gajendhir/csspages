![Variables](./images/variables.svg)

[Home](./readme.md) 

# Variables or Custom Properties in CSS

## Introduction

CSS variables allow us to store a value to some identifier and then use that identifier wherever and whenever that value is needed.

In CSS a variable is an identifier preceeded with two dashes (`--`). To use variables, just..

- Define @property
- Assign values
- Use the value var() function
    -  Fallback values
    -  Invalid values

> Personally, I feel variables are the coolest addition to the CSS stable. 
>
> It has made the task of maintaining and fine-tuning my UI/UX so much easier. I do not have to find and replace every usage of a color value.

## Use @property 

The use of this at-rule is optional. The code works fine even if `@property` definition is not provided.

```CSS
    @property --my-forecolor {
        syntax: <color>;
        inherits: false;
        initial-value: darkblue;
    }
```

The `@property` lets you define the type of the variable, a default value and it allows you to control its inheritance.

## Assign values 

Specify two dashes (`--`) followed by a name for the custom property and assign a valid CSS value after a colon (`:`).

```CSS
:root {
    --my-forecolor: red;
}

.classname {
    --my-forecolor: blue;
}
```

A custom property assigned without the `@property` at-rule always inherits the value of its parent.

### Scope of the Variable

#### Global

A variable declared in the `:root` selector has the **global scope** and can be used throughout the entire document.

#### Local

It has a **local scope** if the variable is declared inside the selector where you want to use it.

> In the code above globally the value of `--my-forecolor` is red, but in the elements having class as `.classname` its value will be blue.

## var() Function

The value in the custom variable can be referenced with the `var()` function.

```CSS
.heading {
    color: var(--my-forecolor);
}
```

### Fallback values

You can add a fallback value to the var() function.

The second argument is the optional fallback value, which is used when the reference value of the variable is *invalid*.

```css
    var(--my-own-color, blue)
```
The fallback value here is *blue*.

The second argument could also reference a variable, like this...

```css
    var(--my-own-color, var(--my-forecolor))
```

and, the second variable could also have a fallback...

```css
    var(--my-own-color, var(--my-forecolor, maroon))
```

### Invalid Custom Properties

When the value assigned to any property is invalid, that declaration is ignored and style is computed as if that declaration did not exist.

>
>```css
>    div {
>        color: blue;
>        background: lightcyan;
>    }
>
>    div {
>        color: 30deg;
>    }
>```
>```html
>    <div>This line is printed</div>
>```
> Here the output would look...
>
> <div style='background:lightcyan'><font color='blue'>This line is printed</font></div>
>

If the value of the variable being referenced is invalid for that property then the `inital` or `inherit`ed value is used.

> ```css
>     :root {
>         --cust-var: 50px;
>     }
> 
>     div {
>         color: blue;
>         background: lightpink;
>     }
> 
>     div {
>         color: var(--cust-var);
>     }
> ```
>```html
>    <div>This line is printed</div>
>```

 Here the output would be printed in `black` - the browser's initial value...
>
> <div style='background:lightpink'><font color='black'>This line is printed</font></div>
> 

 If `@property` at-rule is added, and the value of the variable is invalid, then the `initial-value` of the property will be used.

> ```css
>     @property --cust-var {
>        syntax: '<color>';
>        inherits: false;
>        initial-value: red;
>     }
>
>     :root {
>         --cust-var: 50px;
>     }
> 
>     div {
>         color: blue;
>         background: lightyellow;
>     }
> 
>     div {
>         color: var(--cust-var);
>     }
> ```

 Here the output would be printed in `red` - the initial value defined the property at-rule...

>
> <div style='background:lightyellow'><font color='red'>This line is printed</font></div>
>

[Home](./readme.md)
