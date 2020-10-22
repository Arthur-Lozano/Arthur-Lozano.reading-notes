# Layout

## Building Blocks

- CSS treats each HTML element as if it were in it's own box or container.  There are two types of boxes which are 1. block-level or 2. inline box.



- ex of block-level `<h1>` and `<p>`
- ex of inline elements `<img>` and `<h1>`

* If one block level element were to sit inside another block-level element the outer box would be known as the (parent) element

* It is common practice to group a number of elements together inside a <div>.

> A box may be nested inside several other block-level elements. The containing element is always the direct parent of that element.

* Once again the containing element is ALWAYS the direct parent of that element

- Created using the `a` element
- The text between the `a` tags is shown to the user

> When you are linking to other pages within the same site, you do not need to specify the domain name in the URL. You can use a shorthand known as a relative URL.

# Directory Structure

> On larger websites it's a good idea to organize your code by placing the pages for each different section of the site into a new folder. Folders on a website are sometimes referred to as directories.

- Place pages for each section of a site in different directories
- The main homepage of a sit in HTML is called index.html

> Web servers are usually set up to return the index.html file if no file name is specified.
> EX. Therefore, if you enter examplearts.com it will return examplearts.com/index .html, and examplearts.com/ music will return examplearts .com/music/index.html.

* (URL) Uniform Resource Locator

> Relative URLs can be used when linking to pages within your own website. They provide a shorthand way of telling the browser where to find your files.

* Email Links
- mailto: - Creates a link when clicked on will open the users email program to send an email to a specified email address

- If you want a link to open in a new window use the `Target` attribute Ex (`<a href="http://www.imdb.com" target="_blank"`>)
- The `<a>` element and the and ID tag can be used to link from a hyperlink to anywhere within the page
> Therefore, the href attribute will contain the address for the page (either an absolute URL or a relative URL), followed by the # symbol, followed by the value of the id attribute that is used on the element you are linking to.
> For example, to link to the bottom of the homepage of the website that accompanies this book, you would write: a href="http:/www.htmlandcssbookcom/#bottom"

## Positioning of an element

- Positioning schemes

* Normal Flow - Every block element appears on a new line which causes each item to appear to be lower down the page than the previous one.
* Relative Positioning - Moves the position from where it would be during normal flow to the top, right, bottom or left.
* - Absolute Positioning - Taken out of normal flow (positions element in relation to it's containing element, does not mess with position of surrounding elements because it ignores any space it would have taken up).  Absolute elements move as a user scroll up and down

- Box offset properties tell the browser where the box should be placed within the browser window
- Elements within fixed positions do not affect positioning of surrounding elements

> Floating Elements Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow.

* Whenever an element is removed from normal flow boxes can overlap.  This is where z-index comes into play and allows us developers to decide which object belongs over top of one another.
* In normal flow each block element appears on top of one another
* Relative positioning moves an element in relation to where it would have been in normal flow

### When the position property is given a value of (absolute) the box is taken out of normal flow and no longer affects the position of other elements on the page

> Fixed positioning is a type of absolute positioning that requires the position property to have a value of fixed.

- Fixed position stays in the same position within the browser window.  As a user scrolls it will stay in the same position (fixed)

## Overlapping Elements - Z Index

> When you use relative, fixed, or absolute positioning, boxes can overlap. If boxes do overlap, the elements that appear later in the HTML code sit on top of those that are earlier in the page.
- The z-index property helps to prioritze which object should appear in the front and which should appear in the back.  The higher the number the closer the number appears to the front of the browser window and the lower the number the more it will be overlapped by the higher numbers.

## Floating element

- The float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.

> When you use the float property, you should also use the width property to indicate how wide the floated element should be. If you do not, results can be inconsistent but the box is likely to take up the full width of the containing element (just like it would in normal flow).

- Use float to place elements side by side

## Fixed Width Layouts

> Advantages
> ●● Pixel values are accurate at controlling size and positioning of elements.
> ●● The designer has far greater control over the appearance and position of items on the page than with liquid layouts.
> ●● You can control the lengths of lines of text regardless of the size of the user's window.
> ●● The size of an image will always remain the same relative to the rest of the page.

## Disadvantages

- The Layout designs do not change if the users browser window does.  This can distort or make the content look entirely differently.

# Liquid Layouts

- Preferable 
- Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.

# Layout Grids

- Grid structures are used to help position elements on a page

# Various

> Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.

- Good thing is using pixels values are accurate at controlling the size and position of an element but the bad news is you can end up with huge gaps around the edge of the page along with pixelation problems that could occur when creating, using, or switching devices with the same content.

## Grids may seem like restrictions but in facts come with plenty of benefits.

- Establishes continuity between various pages that might have different designs 
- Helps users have an idea where information will be located on other pages of the site
- Makes the decision to place new content within a site a bit easier
