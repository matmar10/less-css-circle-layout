# less-css-circle-layout

Create LESS CSS circular layout classes similar to a typical grid based layout

## Installation

* Manual inclusion: `@import circle-layout.less`
* Bower: `bower install --save less-css-circle-layout`

## Usage

### In LESS CSS

Create a new circle layout of the specified radius and module size.

```less
.circle-container(@radius, @module-radius, @increment: 1deg, @from-position: 0deg, @to-position: 359deg);
```

Example: generates a `.circle-container-100px` with circle of 200px diameter and modules of 50px wide/high

```css
.circle-container(100px, 25px);
```

### In HTML

Use the generated classes. Here's an example of numbers on a clock face:

```html
<div class="circle-container-100px">
  <div class="circle-center">This will appear dead center</div>
  <div class="circle-position-300deg">1</div>
  <div class="circle-position-330deg">2</div>
  <div class="circle-position-0deg">3</div>
  <div class="circle-position-30deg">4</div>
  <div class="circle-position-60deg">5</div>
  <div class="circle-position-90deg">6</div>
  <div class="circle-position-120deg">7</div>
  <div class="circle-position-150deg">8</div>
  <div class="circle-position-180deg">9</div>
  <div class="circle-position-210deg">10</div>
  <div class="circle-position-240deg">11</div>
  <div class="circle-position-270deg">12</div>
</div>
```

## CSS Class Reference

* **.circle-container-{n}px** - Container of {n} pixels in radius
* **.circle-position-center** - Position a module in the dead center of the circle
* **.circle-position-{n}deg** - Module to be positioned at {n} degrees
* **.align-vertical** - Utility class that sets module line heights identical to their height

