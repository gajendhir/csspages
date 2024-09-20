# Selectors in CSS

## Introduction

Selector is the first part of any CSS rule. This decides in what part of your HTML document the rule will be applied.

## Simple Selectors

Select elements based on name, id, class

## Combinators

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

* `dir`(ltr | rtl) 
* `empty`
* `hover`
* `has`(*selector*)
* `is`()
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

