# “Images” (pp.94-125)

- Create a seperate folder for images
- `<img>` to add an image to a page
- src tells the browser where the image is located
- alt provides a description of the image just in case the image does not render
- (title) element can also be utilized to provide additional information about an image
- Height and Width attributes can be specified for an image
- (alight) attribute can be used to move the image to the left or right.  CSS is utilized in HTML5
- (top,middle,bottom)

## Three rules when creating images

- Save images in the right format
- Save images at the right side
- Use the correct resolution

> The images you use on your website should be saved at the same width and height that you want them to appear on the page.


## Image editing to keep in mind

### Reducing an image
>Example: If your image is 600 pixels wide and 300 pixels tall, you can reduce the size of the image by 50%.
>Result: This will create an image that is quicker to download.

### Increasing an image
> Example: If your image is only 100 pixels wide by 50 pixels tall, increasing the size by 300% would result in poor quality.
> Result: The image will look blurry or blocky.

### Change shape
> Example: If your image is 300 pixels square, you can remove parts of it, but in doing so you might lose valuable information.
> Result: Only some images can be cropped and still make sense.

- Cropping images must be done in the proper way in order to not lose important information that comes along with the image

> When cropping images it is important not to lose valuable information. It is best to source images that are the correct shape if possible.

> JPGs, GIFs, and PNGs belong to a type of image format known as bitmap. They are made up of lots of miniature squares. The resolution of an image is the number of squares that fit within a 1 inch x 1 inch square area.

- The way computers display images

> computers display images at a resolution of 72 pixels per inch (ppi). Images in print materials (such as books and magazines) are made up of tiny circles called dots. These images are usually printed at a resolution of 300 dots per inch (dpi).

- Vector images are different than bitmap images and are resolution independent 
- `<figure>` `<figcaption>` created by HTML5 in order to keep an image and it's caption associated

- There are various tools to edit or create images, I prefer the Adobe tools

# “Color” (pp.246-263)

### Color values
* RGB
* HEX
* Color names

- background-color
>CSS treats each HTML elementas if it appears in a box, and the background-color property sets the color of the background for that box.

-Contrast
> When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.
### It is important for a user to be able to read the text and information that is associated with a website otherwise what would be the point of putting the content on it.

- There is an (opacity) property that can be utilized in CSS 

* Hue
* Saturation
* Lightness

#  “Text” (pp.264-299)

> Serif - Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.

> Sans-Serif - Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.

> Monospace - Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.)

* font-family property allows you to specify the typeface that will be used for any text.
* font-size enables you to specify a specific size of your font.

- bold (appears bold)
- normal (appears at a normal weight)
- italic (appears italic)
- oblique (causes text to appear oblique)

### text-transformation

- uppercase
- lowercase
- capitalize

### text-decoration

- none (This removes any decoration already applied to the text.)
- underline This adds a line underneath the text.
- overline This adds a line over the top of the text.
- line-through This adds a line through words.
- blink This animates the text to make it flash on and off (however this is generally frowned upon, as it is considered rather annoying).

### line-height

> Leading (pronounced ledding) is a term typographers use for the vertical space between lines of text. In a typeface, the part of a letter that drops beneath the baseline is called a descender, while the highest point of a letter is called the ascender. Leading is measured from the bottom of the descender on one line to the top of the ascender on the next.

* letter-spacing (Control spacing between letters)
* word-spacing (Controls spacing between words)

- Text-alignment
* left
* right 
* center
* justify

### vertical alignment
- commonly used with
inline elements such as `<img>`,
`<em>`, or `<strong>` elements.
When used with these elements,
it performs a task very similar to
the HTML align attribute used
on the `<img>` element. The
values it can take are:

- baseline
- sub
- super
- top
- text-top
- middle
- bottom
- text-bottom

### text-indent

* The text - indent property allows you to indent the first line of text within an element.

* text-shadow - allows a shadow to be created for your text (despite no all browsers supporting it)

> You can specify different values for the first letter or first line of text inside an element using
- `:first-letter` 
- `:first-line`
*Technically these are not
properties. They are known as
pseudo-elements.

*You specify the pseudo-element
at the end of the selector, and
then specify the declarations as
you would normally for any other
element.

- :link (This allows you to set styles
for links that have not yet been
visited.)
- :visited (This allows you to set styles for
links that have been clicked on.)

## Responding to Users
- :hover - is applied when a user hovers over an element
- :active - When an element is being activated by a user
- :focus - applied when an element has focus