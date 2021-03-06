# Experiment with CSS Grid Layout

[![licence mit](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](http://hemersonvianna.mit-license.org/)
[![GitHub issues](https://img.shields.io/github/issues/org-victorinox/experiment-css-grid-layout.svg)](https://github.com/org-victorinox/experiment-css-grid-layout/issues)
![GitHub Release Date](https://img.shields.io/github/release-date/org-victorinox/experiment-css-grid-layout.svg)
![GitHub top language](https://img.shields.io/github/languages/top/org-victorinox/experiment-css-grid-layout.svg)
![GitHub repo size](https://img.shields.io/github/repo-size/org-victorinox/experiment-css-grid-layout.svg)
![GitHub All Releases](https://img.shields.io/github/downloads/org-victorinox/experiment-css-grid-layout/total.svg)

## Translations

* [Portuguese - Brazil](translations/pt_BR)

## Browser Support

- Chrome 29+(Enabling flag)
- Firefox 40+(Enabling flag)
- Opera 28+(Enabling flag)
- IE 10+

Only IE 10+ and Edge support Grid Layout. It can be enabled in Chrome through the `Experimental Web Platform features` flag in `chrome://flags`. You can enable it in Firefox using the `layout.css.grid.enabled` flag.

## Terminology

The `fr` unit: This unit is used to specify a fraction of available space. It is meant to be used with `grid-rows` and `grid-columns`.

```html
<div class="grid-container">
  <div class="grid-element item-a">A</div>
  <div class="grid-element item-b">B</div>
  <div class="grid-element item-c">C</div>
  <div class="grid-element item-d">D</div>
  <div class="grid-element item-e">E</div>
  <div class="grid-element item-f">F</div>
</div>
```

```css
.grid-container {
  display: grid;
  grid-template-columns: 200px 10px 0.3fr 10px 0.7fr;
  grid-template-rows: auto 20px auto;
}
```

![fr unit](source/img/unit-fr.png)

### Grid Container

The element on which `display: grid` is applied. It's the direct parent of all the grid items.

```html
<div class="grid-container">
  <div class="grid-item item-1"></div>
  <div class="grid-item item-2"></div>
</div>
```

```css
.grid-container { display: grid; }
```

### Grid Item

Direct children of the `grid container`. Here the `grid-item` elements are grid items, but `grid-subitem` isn't.

```html
<div class="grid-container">
  <div class="grid-item item-1">
    <div class="grid-subitem"></div>
  </div>
  <div class="grid-item item-2"></div>
</div>
```

### Grid Line

The dividing lines that make up the structure of the grid. They can be either vertical (column grid lines) or horizontal (row grid lines) and reside on either side of a row or column. 

![Grid Line](source/img/grid-line.png)

### Grid Track

The space between two adjacent grid lines. You can think of them like the columns or rows of the grid. Here's the grid track between the second and third row grid lines.

![Grid Track](source/img/grid-track.png)

### Grid Cell

The space between two adjacent row and two adjacent column grid lines. It's a single **unit** of the grid. Here's the grid cell between row grid lines 1 and 2, and column grid lines 2 and 3.

![Grid Cell](source/img/grid-cell.png)

### Grid Area

The total space surrounded by four grid lines. A grid area may be comprised of any number of grid cells. Here's the grid area between row grid lines 1 and 3, and column grid lines 1 and 3.

![Grid Area](source/img/grid-area.png)

## Properties

### Properties for the Grid Container

- display
  - grid 
  - inline-grid
- grid-template-columns
- grid-template-rows
- grid-template-areas
- grid-column-gap
- grid-row-gap
- grid-gap
- justify-items
- align-items
- justify-content
- align-content
- grid-auto-columns
- grid-auto-rows
- grid-auto-flow
- grid

### Properties for the Grid Items

- grid-column-start
- grid-column-end
- grid-row-start
- grid-row-end
- grid-column
- grid-row
- grid-area
- justify-self
- align-self

## References 

- [A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [CSS Grid Layout Module Level 1](https://www.w3.org/TR/css-grid-1/)
- [Introducing the CSS Grid Layout](http://www.sitepoint.com/introducing-the-css-grid-layout/)

## Contributing

- Fork it!
- Create your feature branch: `git checkout -b my-new-feature`
- Commit your changes: `git commit -m 'Add some feature'`
- Push to the branch: `git push origin my-new-feature`
- Submit a pull request

## Log

Check [Releases](https://github.com/org-victorinox/experiment-css-grid-layout/releases) for detailed changelog.

## License

[MIT license](http://hemersonvianna.mit-license.org/) © Hemerson Vianna
