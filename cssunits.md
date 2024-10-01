<image src='./images/unitsmeas.png' width='100%'/>


[Home](./readme.md) 

# Units in CSS

Values are regularly used in CSS. These are specified sometimes in [absolute units](#absolute-units) and at other times in [relative units](#relative-units).

CSS provides units for length, angle, frequency and within each category it supports conversion between the different units of measurement.

It is good to have an understanding of the various units or measurement that CSS supports. This allows web developers and designers to work within their comfortable zones.

Below is a list of units supported in CSS...

## Absolute Units

### Length

`cm`, `mm`, `Q`, `in`, `pt`, `pc`, `px`

| Unit | Name |Equivalent to |
|--|--|--|
| cm | Centimeters | 1cm = 37.8px = 1/2.54 of 1in |
| mm | Millimeters | 1mm = 1/10 of 1cm |
| Q | Quarter-millimeters | 1Q = 1/40 of 1cm |
| in | Inches | 1in = 2.54cm = 96px |
| pc | Picas | 1pc = 1/6 of 1in |
| pt | Points | 1pt = 1/72 of 1in |
| px | Pixels | 1px = 1/96 of 1in |

### Angles

`deg`, `grad`, `rad`, `turn`

| Unit | Name |Equivalent to |
|--|--|--|
| deg | Degree | 360deg = 1 full circle |
| grad | Gradian | 400grad = 1 full circle |
| rad | Radian | 6.2832rad = 1 full circle <br/> (π approx = 3.1416) |
| turn | Turn | 1 turn = 1 full cirle |

### Time

`s`, `ms`

| unit | name | equivalent to |
|--|--|--|
| s | second | 1s = 1000ms |
| ms | millisecond | 1ms = 1/1000 of 1s|

### Frequency Units

`Hz`, `kHz`

| unit | name | equivalent to |
|--|--|--|
| Hz | Hertz | 1Hz = 1/1000 of 1 kHz |
| kHz | Kilo Hertz | 1KHz = 1000Hz |

### Resolution Units

`dpi`, `dpcm`, `dppx`


## Relative Units

As the name suggests, the values provided with these type of units are computed in relation to some other value. This other value could some parent element or the viewport itself.

### Font Related

`em`, `ex`, `ch`, `rem`

### Viewport Related

`%`, `vw`, `vh`, `vmin`, `vmax`

### Container Query Related

`cqw`, `cqh`, `cqi`, `cqb`, `cqmin`, `cqmax`

> **Note**
>
> It is common practice to define an absolute value to the container element and then use relative values for the descendants of that element.

[Home](./readme.md)
