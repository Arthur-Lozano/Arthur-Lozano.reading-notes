# Links

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
* Absolute Positioning - Taken out of normal flow (positions element in relation to it's containing element, does not mess with position of surrounding elements because it ignores any space it would have taken up).  Absolute elements move as a user scroll up and down

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


# Functions, Methods, and Objects

* Functions and Methods
- Consist of a series of statements that have been grouped together in order to perfrom a specific task
- A method is the same as a function, except methods are created inside (and are part of an object)
* Objects
- Objects are used to create models of the world around us using data. (Objects are made of properties and methods)
- A method is part of an object
* Built-In Objects - The browser comes with a set of objects that act like a tooklkit for creating interactive web pages.  


# Pair Programming

- 2 minds are better than one

### There are four fundamental skills that help anyone learn a new language

* Listening: hearing and interpreting the vocabulary
* Speaking: using the correct words to communicate an idea
* Reading: understanding what written language intends to convey
* Writing: producing from scratch a meaningful 

- When you ask a function to perform a task later you need to CALL the function.
- Some functions need to be provided information in order to perform a certain task (which is provided within parameters).  Better explained, pieces of information that are passed to a function are called parameters
- When you write a function and expect a response it is known as a (return value)
- When a function is called by it's name the code block will run

* Anonymous functions, which do not have a name and means they cannot be called.  However, they are called as soon as the interpreter comes across them.

### Creating a function 

- Give it a name
- Write the statements needed to achieve it's task within the curly braces

* After declaring a function it can be executed with one line of code (the function named followed by parentheses)
* The same function can be called as many times within the same block of javascript code

## Declraing functions that need information

- Sometimes functions need specific information to perform its tasks and in such situation we need to give it parameters.  Inside the function the parameters work like variables.
> Inside the function those words act like variable names
*  When designing a script it's important to note what information the function will require in order to perform it's task
- Functions can use parameter names within its code block as a variable will be used

# Calling a function with parameters

- Specify the values it should use in the parentheses that follow its name.
- These values are called arguments, and they can be provided as values or variables

## Actual values do not need to be specified when calling a function, variables can be used in their place

> Note the difference between parameters and arguments: Function parameters are the names listed in the function's definition. Function arguments are the real values passed to the function. Parameters are initialized to the values of the arguments supplied.

* Important to note that intrepreter leaves the function when return is used

# Functions can get more than one value using an array



