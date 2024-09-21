[Home](./readme.md) 

# Media Queries in CSS

## Responsive Design

We as website designers are expected to create websites that will deliver optimum user experience for any device that may be used to access the webpage.

The media queries allow us to determine the type of media (screen, printer, speech etc.), size and some capabilities of the media.


### Standard Media Widths for Screens

Standard screen width for responsive designs.

* 320px or 480px (for mobile phones), 
* 768px (for tablets), and 
* 1024px (for small screens, laptops)
* 1920px (for FHD screen computers)

These are the general guidelines that I use when planning my responsive sites.

## Structure of Media Query

The media query has four parts...

`At-Rule` `MediaType` `MediaFeatures` `Operators`

for eg

```css

@media screen and (max-width: 480px) {
    ...
}

@media screen and (max-width: 768px) {
    ...
}

@media screen and (max-width: 1024px) {
    ...
}

@media screen and (min-width: 1024px) {
    ...
}

```

### At-Rule

Media query starts with `@media`

### Media Types

* `all`
* `print`
* `screen`
* `speech`

### Media Features

* `width` (`min-width`, `max-width`)
* `height` (`min-height`, `max-height`)
* `device-width`
* `device-height`
* `orientation`
* `aspect-ratio`
* `device-aspect-ratio`
* `color`
* `color-index`
* `monochrome`
* `resolution`
* `scan`
* `grid`

### Operators

* `and`
* `or` (`,`)
* `not`


## Nested and Complex Queries

Nested queries are supported


[Home](./readme.md)
