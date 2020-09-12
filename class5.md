# Class 5 Notes

* CSS allows you to create rules that control the
way that each individual box (and the contents
of that box) is presented.
* CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.
* link external-css.html HTML
The link element can be used
in an HTML document to tell the
browser where to find the CSS
file used to style the page. It is an
empty element (meaning it does
not need a closing tag), and it
lives inside the head element.
It should use three attributes:
*href
This specifies the path to the
CSS file (which is often placed in
a folder called css or styles).
*type
This attribute specifies the type
of document being linked to. The
value should be text/css.
*rel
This specifies the relationship
between the HTML page and
the file it is linked to. The value
should be stylesheet when
linking to a CSS file.
*An HTML page can use more
than one CSS style sheet. To
do this it could have a link
element for every CSS file it
uses. For example, some authors
use one CSS file to control the
presentation (such as fonts and
colors) and a second to control
the layout.
* You can also include CSS rules
within an HTML page by placing
them inside a style element,
which usually sits inside the
head element of the page.


# How CSS rules cascade 

*If there are two or more rules
that apply to the same element,
it is important to understand
which will take precedence.
LAST RULE
If the two selectors are identical,
the latter of the two will take
precedence. Here you can see
the second i selector takes
precedence over the first.
SPECIFICITY
If one selector is more specific
than the others, the more
specific rule will take precedence
over more general ones. In this
example:
h1 is more specific than 
p b is more specific than p
p#intro is more specific than p
IMPORTANT
You can add !important after
any property value to indicate
that it should be considered
more important than other rules
that apply to the same element.
Understanding how CSS rules
cascade means you can write
simpler style sheets because
you can create generic rules
that apply to most elements and
then override the properties on
individual elements that need to
appear differently.

# Colors

* RGB, Color names, Hex codes, HSLA
* HSLA, CSS3 introduces an entirely new and intuitive
way to specify colors using hue, saturation,
and lightness values.
* hue
Hue is the colloquial idea of
color. In HSL colors, hue is often
represented as a color circle
where the angle represents the
color, although it may also be
shown as a slider with values
from 0 to 360.
saturation
Saturation is the amount of
gray in a color. Saturation is
represented as a percentage.
100% is full saturation and 0%
is a shade of gray.
ligh tness
Lightness is the amount of
white (lightness) or black
(darkness) in a color. Lightness
is represented as a percentage.
0% lightness is black, 100%
lightness is white, and 50%
lightness is normal. Lightness
is sometimes referred to as
luminosity.
* hue
This is expressed as an angle
(between 0 and 360 degrees).
saturation
This is expressed as a
percentage.
lightness
This is expressed as a
percentage with 0% being white,
50% being normal, and 100%
being black.
--
* CSS treats each HTML element
as if it appears in a box, and the
background-color property
sets the color of the background
for that box.
* Contrast
When picking foreground and background
colors, it is important to ensure that there is
enough contrast for the text to be legible.
- Text is harder to read when
there is low contrast between
background and foreground
colors.
- Text is easier to read when
there is higher contrast between
background and foreground
colors.
- For long spans of text, reducing
the contrast a little bit improves
readability.
* The CSS3 rgba property allows
you to specify a color, just like
you would with an RGB value,
but adds a fourth value to
indicate opacity. This value is
known as an alpha value and is
a number between 0.0 and 1.0
(so a value of 0.5 is 50% opacity
and 0.15 is 15% opacity). The
rgba value will only affect the
element on which it is applied
(not child elements).
