---
title: Borders
path: utilities/borders
status: Stable
status_issue: 'https://github.com/github/design-systems/issues/72'
source: 'https://github.com/primer/css/tree/master/src/utilities/borders.scss'
bundle: utilities
---

Utilities for borders, border radius, and box shadows.

{:toc}

## Default border

The default border utility applies a solid, 1px border, with a default gray color.

```html
<div class="border">
  .border
</div>
```

Borders can be applied to a specific edge or to the Y axis.

```html
<div class="d-flex mb-3">
  <div class="border-left col-3">
    .border-left
  </div>
  <div class="border-top col-3">
    .border-top
  </div>
  <div class="border-bottom col-3">
    .border-bottom
  </div>
  <div class="border-right col-3">
    .border-right
  </div>
</div>
<div class="border-y">
  .border-y
</div>
```

Remove borders from all sides or a single side with `.border-0`, `.border-top-0`, `.border-right-0`, `.border-bottom-0`, `.border-left-0`.

```html
<div class="Box border-top-0">
  .border-top-0
</div>
```

## Border colors

Override default border colors with blue, green, red, purple, yellow, and gray border color utilities.

```html
<div class="border border-blue mb-2">
  .border-blue
</div>
<div class="border border-blue-light mb-2">
  .border-blue-light
</div>
<div class="border border-green mb-2">
  .border-green
</div>
<div class="border border-green-light mb-2">
  .border-green-light
</div>
<div class="border border-red mb-2">
  .border-red
</div>
<div class="border border-red-light mb-2">
  .border-red-light
</div>
<div class="border border-purple mb-2">
  .border-purple
</div>
<div class="border border-yellow mb-2">
  .border-yellow
</div>
<div class="border border-gray-light mb-2">
  .border-gray-light
</div>
<div class="border border-gray-dark mb-2">
  .border-gray-dark
</div>
```

### Borders with alpha transparency

Use `border-black-fade` to add an rgba black border with an alpha transparency of `0.15`. This is useful when you want a border that tints the background color. The shade of black we use matches the hue of the GitHub dark header and our gray color palette: `rgba(27,31,35, 0.15)`.

```html
<div class="border border-black-fade bg-blue-light p-2 mb-2">
  .border-black-fade .bg-blue-light
</div>
<div class="border border-black-fade bg-red-light p-2 mb-2">
  .border-black-fade .bg-red-light
</div>
```

On dark backgrounds use `border-white-fade` instead. It adds an rgba white border with an alpha transparency of `0.15`.

```html
<div class="bg-gray-dark text-white p-3">
  <div class="border border-white-fade p-2">
    .border-white-fade
  </div>
</div>
```

Use `.border-white-fade-xx` to add a white border with various levels of alpha transparency.

```html
<div class="bg-gray-dark text-white p-3 mb-3">
  <div class="border-bottom border-white-fade-15 p-2 mb-2">
    .border-white-fade-15
  </div>
  <div class="border-bottom border-white-fade-30 p-2 mb-2">
    .border-white-fade-30
  </div>
  <div class="border-bottom border-white-fade-50 p-2 mb-2">
    .border-white-fade-50
  </div>
  <div class="border-bottom border-white-fade-70 p-2 mb-2">
    .border-white-fade-70
  </div>
  <div class="border-bottom border-white-fade-85 p-2 mb-2">
    .border-white-fade-85
  </div>
</div>
<div class="bg-blue text-white p-3">
  <div class="border-bottom border-white-fade-15 p-2 mb-2">
    .border-white-fade-15
  </div>
  <div class="border-bottom border-white-fade-30 p-2 mb-2">
    .border-white-fade-30
  </div>
  <div class="border-bottom border-white-fade-50 p-2 mb-2">
    .border-white-fade-50
  </div>
  <div class="border-bottom border-white-fade-70 p-2 mb-2">
    .border-white-fade-70
  </div>
  <div class="border-bottom border-white-fade-85 p-2 mb-2">
    .border-white-fade-85
  </div>
</div>
```

## Border style

Use `border-dashed` to give an element a dashed border.

```html
<div class="border border-dashed p-2">
  .border-dashed
</div>
```

## Rounded corners

Use the following utilities to add or remove rounded corners: `rounded-0` removes rounded corners, `rounded-1` applies a border radius of 3px, `rounded-2` applies a border radius of 6px. `.circle` applies a border radius of 50%, which turns square elements into perfect circles.

```html
<div class="Box rounded-0 mb-2">
  .rounded-0
</div>
<div class="border rounded-1 mb-2">
  .rounded-1
</div>
<div class="border rounded-2 mb-2">
  .rounded-2
</div>
<div class="border circle p-3" style="width: 100px; height: 100px;">
  .circle
</div>
```

You can also add rounded corners to each edge (top, right, bottom, left) with the following utilities:

```html
<div class="border rounded-top-1 mb-2">
  .rounded-top-1
</div>
<div class="border rounded-right-1 mb-2">
  .rounded-right-1
</div>
<div class="border rounded-bottom-1 mb-2">
  .rounded-bottom-1
</div>
<div class="border rounded-left-1 mb-2">
  .rounded-left-1
</div>
```

## Responsive borders

Top, right, bottom, and left border utilities are can be used responsively to add or remove borders to an element at different screensizes.

```html
<div class="border-top border-sm-right border-md-bottom border-lg-top-0">
  .border-top-0
</div>
```
