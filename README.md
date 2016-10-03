# Responsive Grid
Responsive grid is a minimal implementation of a 12-column mobile-first responsive grid. It is based on code from the [w3schools.com Responsive Web Design tutorial](http://www.w3schools.com/css/css_rwd_intro.asp).

# Usage
Simply include `grid.css` in your HTML document. To define the number of columns you want an element to take up, give it the `col-[x]` class, where `x` is a number from 1 to 12. If you want it to take up that many columns only on medium screens (<768px), use the `col-m-[x]` class. For small screens (<414px), use `col-s-[x]`.

## Example
<script async src="//jsfiddle.net/x3f56bLp/3/embed/html,result/"></script>

# Installation
`grid.css` is served on Github pages. To include it in your html file, use:

```html
<link rel="stylesheet" type="text/css" href="https://jdormit.github.io/responsive-grid/grid.css">
```

To download the file (in terminal):
`wget https://jdormit.github.io/responsize-grid/grid.css`

Or simply <a href="https://jdormit.github.io/responsive-grid/grid.css" download>download from here</a>
