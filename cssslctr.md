[Home](./readme.md) 

# Selectors in CSS

## Introduction

Selector is the first part of any CSS rule. This decides in what part or section of your HTML document the rule will be applied.

```css

selector {
    property: value;
    ....
}

```

## Simple Selectors

Select elements based on name, id, class

## Combinators

A combinator is a combination of two or more selectors used together. Combinators are used define the specificity of the selector.

### Descendant Selector (space)

eg
```css
div p {
    ...
}
```
This will select all `p`s *under* all `div`s. `p`s in any child of the `div`s will also be included.

### Child Selector (>)

eg
```css
div > p {
    ...
}
```
This will select all `p`s *directly under* all `div`s. `p`s nested inside any child of `div` will not be included.

### Adjacent Sibling Selector (+)

eg
```css
div + p {
    ...
}
```
This will select `p`s that are *immediately* after `div`s - at the same level. No parent or child will be included.

### General Sibling Selector (~)

eg
```css
div ~ p {
    ...
}
```
This will select `p`s that are *anywhere* after `div`s - at the same level. No parent or child will be included.

## Pseudo-classes

Pseudo-classes are selectors that are recognized in the browser without explicitly being defined in the web-page.

A pseudo-class can used by adding `:` before it.

eg
```css
  a:active          /* active links */
  div:hover         /* when mouse hovers over the <div> */
  div:first-child   /* the first child inside the <div> */
```

### List of Pseudo-classes

* `:active`
* `:any-link`
* `:dir`(ltr|rtl) 
* `:empty`
* `:has`(*selector*)
* `:hover`
* `:is`(*selector*)
* `:lang`(*language*)
* `:link`
* `:not`(*selector*)
* `:root`
* `:state`(*identifier*)
* `:target`
* `:visited`
* `:where`(*selector*)

/* for child */

* `:first-child`
* `:last-child`
* `:nth-child`(*position*)
* `:nth-last-child`(*position*)
* `:only-child`

/* for of-type */

* `:first-of-type`
* `:last-of-type`
* `:nth-of-type`(*position*)
* `:nth-last-of-type`(*position*)
* `:only-of-type`

/* Input */

* `:checked`
* `:disabled`
* `:enabled`
* `:focus`
* `:focus-visible`
* `:in-range`
* `:inderminate`
* `:invalid`
* `:optional`
* `:out-of-range`
* `:read-only`
* `:read-write`
* `:required`
* `:valid`

## CSS Pseudo Elements

Pseudo Elements are elements that the browser recognizes even though they are not defined in the web-page.

* `::after`
* `::before`
* `::file-selector-button`
* `::first-letter`
* `::first-line`
* `::grammar-error`
* `::marker`
* `::placeholder`
* `::selection`
* `::spelling-error`
* `::target-text`
* `::backdrop`
* `::cue`
* `::highlight`
* `::part`
* `::slotted`
* `::view-transition`
* `::view-transition-image-pair()`
* `::view-transition-group()`
* `::view-transition-new()`
* `::view-transition-old()`



[Home](./readme.md)
