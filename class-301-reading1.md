# RESPONSIVE WEB DESIGN and FLOATS

### Responsive Web Design

- In the UK there are more mobile devices than people
- Responsive web design is the process of building website that will work on every device and screen size
- Responsive web design is designed to please everyone no matter what device they are utilizing to view it
- Responsive web design term was coined by Ethan Marcotte
> Responsive design websites continually and fluidly change based on different factors, such as viewport width
> Adaptive websites are built to a group of preset factors. A combination of the two is ideal, providing the perfect formula for functional websites. Which term is used specifically doesn’t make a huge difference.
- Mobile development which usually involves building another website on a different domain specifically for mobile users which can cause problems.
- As of now responsive web developent is the most popular web development
> favoring design that dynamically adapts to different browser and device viewports, changing layout and content along the way. *This solution has the benefits of being all three, responsive, adaptive, and mobile.

## Flexible Layouts

- Responsive web design is broken down into three components
* Flexible layouts
> The first part, flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width. Flexible grids are built using relative length units, most commonly percentages or em units.
* Media Queries
* Flexible media

- Flexible layouts do not use fixed measurements (such as pixels and inches) because that would restrict it from being able to adjust according to new devices needs.  Viewport height and width tend to change from device to device.

## Relative Viewport Lengths

> CSS3 introduced some new relative length units, specifically related to the viewport size of the browser or device. These new units include vw, vh, vmin, and vmax. Overall support for these new units isn’t great, but it is growing. In time they look to play a large roll in building responsive websites.

- vw - Viewports width
- vh - Viewports height
- vmin - Minimum of the viewport’s height and width
- vmax - Maximum of the viewport’s height and width

> With the growth in mobile Internet usage comes the question of how to build websites suitable for all users. The industry response to this question has become responsive web design, also known as RWD.

## Media queries 
 > There are a couple different ways to use media queries, using the @media rule inside of an existing style sheet, importing a new style sheet using the @import rule, or by linking to a separate style sheet from within the HTML document. Generally speaking it is recommend to use the @media rule inside of an existing style sheet to avoid any additional HTTP requests.

 > built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example. Being able to apply uniquely targeted styles opens up a world of opportunity and leverage to responsive web design.

- The @media rule inside of an existing stylesheet is the preferred method of use
- Media types - all, screen, print, tv, and braille (default media type screen)

### Logical operators in media queries
- and (allowing extra condition to be added)
- not (specifies any query but the one mentioned)
- only (specifies only the query mentioned and is a new operator)


# Height and width media features

> One of the most common media features revolves around determining a *height or width for a device or browser viewport*. The height and width may be found by using the height and width media features. Each of these media features may then also be prefixed with the min or max qualifiers, building a feature such as min-width or max-width.

- Within responsive design the most commonly used features include min-width and max-width. These help build responsive websites on desktops and mobile devices equally, avoiding any confusion with device features.

- Oritentation media feature determines if a device is in a landscape or portrait orientation.
- Aspect Ratio Media Features
- Pixel Ratio Media Features
- Breakpoints should only be used when a website starts to actually break, look bad, or the experience is being altered. Something to keep in mind is that new devices and resolutions are being created all the time and keeping up with them could be almost impossible.

* Mobile first approach with media queeries is great.
- Use styles that target smallter viewports by default and then use media queries to add styles as the viewport grows.
- As mentioned previously with the growing number of mobile users in the UK alone, targeting mobile first will help keep the website useful.


* Downloading unnecessary media assets can also be stopped with the help of media queries.
- Maybe taking out the background animation on a mobile device and instead putting a background color.  This would reduces heavy loading and possibly save battery life.

### Viewport

- Apple invented the viewport meta tag to help mobile devices indetify the viewport size, scale and resolution of a website.

> Turning off the ability to scale a website is a bad idea. It harms accessibility and usability, preventing those with disabilities from viewing a website as desired.

# Float

- Float's sister property is clear, an element that has the clear property set won't move up adjacent to the float like the float would like (Also being a common problem for some)
* Techniques for clearing floats
- `<div style="clear: both;"></div>`
- The overflow method
- The Easy Clearing Method uses a clever CSS pseudo selector (:after) to clear floats.
- Pushdown 

> A common example is an image sticking out of the main content push the sidebar down below.
> Quick fix: Make sure you don’t have any images that do this, use overflow: hidden to cut off excess.
> The 3px Jog is when text that is up next to a floated element is mysteriously kicked away by 3px like a weird forcefield around the float. Quick fix: set a width or height on the affected text.

- Using float to fix elements such as block elements `div`

> Floats create alternate flows. This is the hardest part to understand. And once you introduce them, you then need to write your code so that it accounts for up to three flows: normal, left and right. This is a whole new set of rules, as opposed to manipulating the width of elements or their positioning.

- Floats along with the clear property can be explained below to gie a more clear picture and idea of the dynamics within a div 

- Using no floats = no order on a busy 3 lane one way street
- Using float left and right puts an item on the left and right; therefore, allowing other cars to take up the spaces between (Normal flow of elements)

> “Clear” allows elements to specify where they should align in comparison to the floated elements.
- “Clear: left” tells each person floating left that they should align themselves behind the first element that is floated left.

- One of the most frequent uses of the clear property is “clear:both”. This allows you to reset the flow of elements, as opposed to continuing to maintain a right, left and normal flow.
- “Clear: both” acknowledges that there may be up to three flows, and blocks the passage of any element that follows.

- `:after` often used to clear floats

- box-sizing: border-box;

## Smacss

- Style Guide for css
- Scalable and modular architecture for css

> It is an attempt to document a consistent approach to site development when using CSS. And really, who isn’t building a site with CSS these days?!



Reference (https://learn.shayhowe.com/advanced-html-css/responsive-web-design/)
Reference (https://css-tricks.com/all-about-floats/)
Reference (https://www.freecodecamp.org/news/css-floats-explained-by-riding-an-escalator-57fa55232333/)
Reference (https://css-tricks.com/dont-overthink-it-grids/)
Reference (http://smacss.com/)