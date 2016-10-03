# Responsive Grid
Responsive grid is a minimal implementation of a 12-column mobile-first responsive grid. It is based on code from the [w3schools.com Responsive Web Design tutorial](http://www.w3schools.com/css/css_rwd_intro.asp).

# Usage
Simply include `grid.css` in your HTML document. To define the number of columns you want an element to take up, give it the `col-[x]` class, where `x` is a number from 1 to 12. You can also specify different widths for different screen sizes. `col-2` will take up 2 columns on desktop screens, and all 12 columns on smaller screens. `col-m-2` will take up 2 columns on desktop and tablet screens, and all 12 columns on mobile screens. `col-s-2` will take up 2 columns on all screen sizes mobile and larger. These can be combined - `col-4 col-m-6 col-s-8` will take up 4 columns on desktop screens, 6 columns on tablet screens, and 8 columns on mobile screens.

You can push elements to the right a certain number of columns using the `push-[x]` classes, where `x` is the number of columns to push the content. These are also separated by size, so `push-2` will push the content 2 columns to the right on desktop screens, `push-m-2` will do the same on desktop and tablet screens, and `push-s-2` will do the same on mobile screens and larger. These can be combined, so, for instance, `push-2 push-m-3 push-s-4` will push the content over 2 columns on desktop screens, 3 columns on tablet screens, and 4 columns on modile screens.

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
    <div class="col-s-12 col-m-6 col-3">
        This text will take up a whole row on screen sizes < 414px,
    </div>
    <div class="col-s-12 col-m-6 col-3">
        half a row on screen sizes between 415px and 768px,
    </div>
    <div class="col-s-12 col-m-6 col-3">
        and a quarter of a row
    </div>
    <div class="col-s-12 col-m-6 col-3">
        on larger screens.
    </div>
</div>
<div class="row">
    <div class="col-s-4 push-s-4">
        This text will take up the middle 4 columns on all screens.
    </div>
</div>
<div class="row">
    <div class="col-2 push-2 col-m-3 push-m-1 col-s-4">
        This text will be 2 columns wide separated by 2 empty columns on large screens,
    </div>
    <div class="col-2 push-2 col-m-3 push-m-1 col-s-4">
        3 columns wide separated by 1 empty column on medium screens,
    </div>
    <div class="col-2 push-2 col-m-3 push-m-1 col-s-4">
        and 4 columns wide with no separation on small screens.
    </div>
</div>
```

This example is reproduced in `example.html`, which is hosted [here](https://jdormit.github.io/responsive-grid/example.html).

If you want to play around with it yourself, check out the [JSFiddle](https://jsfiddle.net/hfndm0cf/).

# Installation
`grid.css` is served on Github pages. To include it in your html file, use:

```html
<link rel="stylesheet" type="text/css" href="https://jdormit.github.io/responsive-grid/grid.css">
```

To download the file (in terminal):

`wget https://jdormit.github.io/responsize-grid/grid.css`

Or simply <a href="https://jdormit.github.io/responsive-grid/grid.css" download>download from here</a>.
