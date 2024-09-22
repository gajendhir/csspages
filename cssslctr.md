[Home](./readme.md) 

# Selectors in CSS

## Introduction

Selector is the first part of any CSS rule. This decides in what part of your HTML document the rule will be applied.

## Simple Selectors

Select elements based on name, id, class

## Combinators

Selectors are combined to form combinators. Combinators are used define the specificity of the selector.

### Descendant Selector (space)

### Child Selector (>)

### Adjacent Sibling Selector (+)

### General Sibling Selector (~)



## Pseudo-classes

Select based on some state of an element

### Anchor Pseudo-classes

* `a:any-link`
* `a:link`
* `a:visited`
* `a:hover`
* `a:active`

### CSS Pseudo-classes

Pseudo-classes are classes that are recognized in the browser without explicitly being defined in the web-page 

* `dir`(ltr | rtl) 
* `empty`
* `hover`
* `has`(*selector*)
* `is`(*selector*)
* `lang`(*language*)
* `not`(*selector*)
* `root`
* `target`
* `where`(*selector*)

/* for child */

* `first-child`
* `last-child`
* `nth-child`
* `nth-last-child`
* `only-child`

/* for of-type */

* `first-of-type`
* `last-of-type`
* `nth-of-type`
* `nth-last-of-type`
* `only-of-type`

/* Input */

* `checked`
* `disabled`
* `enabled`
* `focus`
* `focus-visible`
* `in-range`
* `inderminate`
* `invalid`
* `optional`
* `out-of-range`
* `read-only`
* `read-write`
* `required`
* `valid`

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
