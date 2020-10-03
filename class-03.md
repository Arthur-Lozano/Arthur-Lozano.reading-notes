# Week Three Notes

## Lists

* Numbered Lists
* Bullet Lists
* Definition lists

- Ordered lists - Each item in a list is numbered.
- Unordered lists - lists that begin with a bullet point.
- Definition lists - Lists set up with terms along with definitions to go along with these terms.

* `<ol>` Creates an ordered list and each item within the list is placed within `<li>`, both of these tags must be accompanied by closing tags.
* `<ul>` Creates an unordered list and just like ordered lists will utilize `<li>` items to display the content with each unordered list

## Other less common lists but still utilized

* `<dl>` definition list is created with this tag, inside the dl tag you will usually find the two below tags of (dt,dd)
* `<dt>` used to contain the term being defined with the `<dl>`
* `<dd>` this tag actually holds the definition.

- Nested Lists
* A second list can be placed witin a `<li>` to create a sub list or nested list

# Boxes

* Controlling sizes of boxes
* Box models for borders, margin and padding
* Displaying and hiding boxes

## CSS treats each HTML element as if it lives in its own box

* By default a box size is just as big as the content needs

### Box size options

- Width
- Height
- Specifying size of boxes use (px, em, %)

> The most popular ways to specify the size of a box are to use pixels, percentages, or ems. Traditionally, pixels have been the most popular method because they allow designers to accurately control their size. When you use percentages, the size of the box is relative to the size of the browser window or, if the box is encased within another box, it is a percentage of the size of the containing box. When you use ems, the size of the box is based on the size of text within it. Designers have recently started to use percentages and ems more for measurements as they try to create designs that are flexible across devices which have different-sized screens.
