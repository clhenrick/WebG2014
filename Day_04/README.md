WebG2014
========

Bootcamp Web G Section 2014


Day 4: CSS Positioning and Floats
=========================

## Positioning

- The CSS positioning properties allow you to position an element. It can also place an element behind another, and specify what should happen when an element's content is too big.

- Elements can be positioned using the top, bottom, left, and right properties. However, these properties will not work unless the position property is set first. They also work differently depending on the positioning method.


**There are four different positioning methods:**


###Static Positioning###
- HTML elements are positioned static by default. A static positioned element is always positioned according to the normal flow of the page.

- Static positioned elements are not affected by the top, bottom, left, and right properties.


###Fixed Positioning###
- An element with fixed position is positioned relative to the browser window.

- It will not move even if the window is scrolled:

Example:
`p.pos_fixed {
    position: fixed;
    top: 30px;
    right: 5px;
}`

Try out: [CSS Code](http://www.w3schools.com/css/tryit.asp?filename=trycss_position_fixed)

- Fixed positioned elements are removed from the normal flow. The document and other elements behave like the fixed positioned element does not exist.

- Fixed positioned elements can overlap other elements.


###Relative Positioning###
- A relative positioned element is positioned relative to its normal position.

Example: `h2.pos_left {
    position: relative;
    left: -20px;
}`

h2.pos_right {
    position: relative;
    left: 20px;
}`

Try out: [CSS Code](http://www.w3schools.com/css/tryit.asp?filename=trycss_position_relative)

- The content of relatively positioned elements can be moved and overlap other elements, but the reserved space for the element is still preserved in the normal flow.

Example:
`h2.pos_top {
    position: relative;
    top: -50px;
}`

Try out: [CSS Code](http://www.w3schools.com/css/tryit.asp?filename=trycss_position_relative2)

- Relatively positioned elements are often used as container blocks for absolutely positioned elements.

###Absolute Positioning###

- An absolute position element is positioned relative to the first parent element that has a position other than static. If no such element is found, the containing block is `<html>:

Example:
`h2 {
    position: absolute;
    left: 100px;
    top: 150px;
}`

Try out: [CSS Code](http://www.w3schools.com/css/tryit.asp?filename=trycss_position_absolute)

- Absolutely positioned elements are removed from the normal flow. The document and other elements behave like the absolutely positioned element does not exist.

- Absolutely positioned elements can overlap other elements.


###Overlapping Elements###

- When elements are positioned outside the normal flow, they can overlap other elements.

- The z-index property specifies the stack order of an element (which element should be placed in front of, or behind, the others).

- An element can have a positive or negative stack order:
Example:
`img {
    position: absolute;
    left: 0px;
    top: 0px;
    z-index: -1;
}`

Try out: [CSS Code](http://www.w3schools.com/css/tryit.asp?filename=trycss_zindex)

- An element with greater stack order is always in front of an element with a lower stack order.

##What is CSS Float?

- With CSS float, an element can be pushed to the left or right, allowing other elements to wrap around it.

- Float is very often used for images, but it is also useful when working with layouts.


###How Elements Float
- Elements are floated horizontally, this means that an element can only be floated left or right, not up or down.

- A floated element will move as far to the left or right as it can. Usually this means all the way to the left or right of the containing element.

- The elements after the floating element will flow around it.

- The elements before the floating element will not be affected.

- If an image is floated to the right, a following text flows around it, to the left:

Example:
`img {
    float: right;
}`
Try out: [CSS Code](http://www.w3schools.com/css/tryit.asp?filename=trycss_float)

###Floating Elements Next to Each Other

- If you place several floating elements after each other, they will float next to each other if there is room.

- Here we have made an image gallery using the float property:

`.thumbnail {
    float: left;
    width: 110px;
    height: 90px;
    margin: 5px;
}`

Try out: [CSS Code](http://www.w3schools.com/css/tryit.asp?filename=trycss_float_elements)


###Turning off Float - Using Clear



## references:
- MDN reference: https://developer.mozilla.org/en-US/docs/Web/CSS/Reference
- css tricks: http://css-tricks.com/pseudo-class-selectors/
- more css tricks: http://css-tricks.com/pseudo-element-roundup/

