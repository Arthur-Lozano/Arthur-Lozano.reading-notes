# Readings: CSS GRID

## Regex Tutorial

> Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern (i.e. a specific sequence of ASCII or unicode characters).
### Fields of application
- validation to parsing/replacing strings
- passing through translating data to other formats and web scraping.
- Can be utilized in almost all programming languages

## CSS Grid Reference

> CSS Grid Layout is the most powerful layout system available in CSS. It is a 2-dimensional

> You work with Grid Layout by applying CSS rules both to a parent element (which becomes the Grid Container) and to that element’s children (which become Grid Items).

- Parents become the container
- Children become the element's
- display
- grid-column-start
- grid-column-end
- grid-row-start
- grid-row-end
- grid-template-columns
- grid-template-rows
* justify-self
- start – aligns the grid item to be flush with the start edge of the cell
- end – aligns the grid item to be flush with the end edge of the cell
- center – aligns the grid item in the center of the cell
- stretch – fills the whole width of the cell (this is the default)

* grid - used to set all the following properties with one declaration: grid-template-rows, grid-template-columns, grid-template-areas, grid-auto-rows, grid-auto-columns, and grid-auto-flow (Note: You can only specify the explicit or the implicit grid properties in a single grid declaration).


## Responsive design with CSS Grid

> In the same way that flexbox gave us a way to layout block elements next to each other, CSS grid lets us not only arrange elements in a row or a column, but in multiple rows and columns. Finally two dimensional layouts are becoming simpler!

- 2 dimenstional layouts made simple

- Grid allows us the ability to control that aspect ratio of each element better to dynamically fit various viewports easier
- ex. `grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));`
