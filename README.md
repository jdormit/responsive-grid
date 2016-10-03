# Responsive Grid
Responsive grid is a minimal implementation of a 12-column mobile-first responsive grid. It is based on code from the [w3schools.com Responsive Web Design tutorial](http://www.w3schools.com/css/css_rwd_intro.asp).

# Usage
Simply include `grid.css` in your HTML document. To define the number of columns you want an element to take up, give it the `col-[x]` class, where `x` is a number from 1 to 12. If you want it to take up that many columns only on medium screens (<768px), use the `col-m-[x]` class. For small screens (<414px), use `col-s-[x]`.

## Example
```html
<link rel="stylesheet" type="text/css" href="https://jdormit.github.io/responsive-grid/grid.css">
<div class="row">
    <div class="col-12">
        This text will take up the whole row on all screen sizes.
    </div>
</div>
<div class="row">
    <div class="col-m-12 col-6">
        This text will take up a whole row on screen sizes < 768px,
    </div>
    <div class="col-m-12 col-6">
        but only half a row on larger screens.
    </div>
</div>
<div class="row">
    <div class="col-s-12 col-m-4 col-3">
        This text will take up a whole row on screen sizes < 414px,
    </div>
    <div class="col-s-12 col-m-4 col-3">
        a fourth of a row on screen sizes between 415px and 768px,
    </div>
    <div class="col-s-12 col-m-4 col-3">
        and a third of a row
    </div>
    <div class="col-s-12 col-m-4 col-3">
        on larger screens.
    </div>
</div>
```

If you want to play around with it yourself, check out the [JSFiddle](https://jsfiddle.net/x3f56bLp/4/).

# Installation
`grid.css` is served on Github pages. To include it in your html file, use:

```html
<link rel="stylesheet" type="text/css" href="https://jdormit.github.io/responsive-grid/grid.css">
```

To download the file (in terminal):

`wget https://jdormit.github.io/responsize-grid/grid.css`

Or simply <a href="https://jdormit.github.io/responsive-grid/grid.css" download>download from here</a>.
