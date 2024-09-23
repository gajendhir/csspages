# Coordinate System in CSS

## Dimensions

### x-cordinate

indicates the location on the horizontal axis

### y-cordinate

indicates the location on the vertical axis

### z-cordinate

indicates the position along views - to - screen axis.


## Cordinate System 

CSSOM support 4 cordinate systems...

### Offset

Offset is the position on the element being considered.

### Viewport

Viewport is the entire viewing area in which the document is presented.

### Page

Page is the entire rendered document. Any cordinate on the page cordinate system will always be same, no matter how much it has been scrolled.

### Screen

Screen is the entire physical device where the document is presented. A single point on the Screen will correspond to the different points on the Viewport if the Viewport is moved.

## Cordinates in Event Handling

### MouseClick Event

* `MouseClick.OffsetX` and `MouseClick.OffsetY`
* `MouseClick.ClientX` and `MouseClick.ClientY`
* `MouseClick.PageX` and `MouseClick.PageY`
* `MouseClick.ScreenX` and `MouseClick.ScreenY`

### Touch Event

* `Event.ClientX` and `Event.ClientY`
* `Event.PageX` and `Event.PageY`
* `Event.ScreenX` and `Event.ScreenY`

## Transform the cordinates

The cordinates of certain elements can be transformed. The transform operations supported are...

* `transform-origin`
* `rotate`
* `scale`
* `translate`
* `skew`
* `perspective`

Some of the transformations support operations in 3d also.