# Markup

### When creating a web page developers use tags also known as markup to the contents of the webpage in order to show web browsers the appropriate structure of the webpage.

## Structural markup

### Elements ussed to describe both heading and paragraph 
## Semantic markup

### Provides extra informatione, for example where extra emphasis is placed in a sentence

## HTML has 6 levels of headings
### `<h1>` is used for main headings and `<h2>` is used for subheadings and below that is `<h3>` and it continues to `<h6>`.
### Basically, h1 tags are displayed by the browser as the largest text and h6 as the smallest text.

## Some basic tags and also necessary tags within html are listed below

* `<p>` P tags are for creating paragraphs within your website.
* `<i>` This tag is used to put your text into an italic format.
* `<sup>` Used to contain characters that are meant to be superscript for example mathematical concepts like raising a number to a power.
* `<sub>` Used for characters that should be subscript, commonly used for foot notes or chemical formulas
* `<br />` Line break tag
* `<hr />` Horizontal rule is used to create breaks between themes

## White Space 

### in order to make code easer to read developers usually add extra spaces or start elements on another line.  When a browser comes across two or more spaces next to one another it only displays once space.  Also, if it comes across a line break it w ill treat that as one space too (known as white space collapsing).
> You will often see that web page authors take advantage of white space collapsing to indent their code in order to make it easier to follow.

# Semantic markup is intended to affect the structure of your page but instead are utilized to add extra information

* `<strong>` Puts text in bold
* `<em>` Will put text in italic
* `<blockquote>` Used for longer quotes that take up an entire paragraph
* `<q>` Used for shorter quotes that tend to sit within a paragraph
* `<abbr>` Used for an abbreviation or acronym
* `<cite>` Is used when referencing professional work such as a book, paper, or film
* `<dfn>` Used to indicate the defining instance of a new term
* `<address>` The address element is used to contain the contact details for the author of the page
* `<ins>` Ins element is ussed to show content that has been inserted into an element
* `<del>` Can be used to show text that has been deleted from an element 
* `<s>` This element shows something that is no longer relevant to the page but should not be deleted and will have a line drawn through it


# CSS allows us to change the way our content appears through the browser

## After learning how to write CSS rules, the next step is learning the various properties that are available to us
## The key to understanding CSS is to imagine that there is an invisible box around each element

### CSS allows us to create rules that control the way each individual box is presented.  
### CSS helps us to create borders around any boxes, specify their width and heigh, color, and even manipulate certain characteristics of the text or content within said boxes.

# Examples

> Width and height - Borders (color, width, and style), Background color and images, Position in the browser window.

> Text - Typeface, Size, Color, Italics, bold, uppercase, lowercase, small-caps

### There are also specific ways to style an element such as lists, tables and forms.

# CSS works by associating rules with HTML elements.  These rules govern how the content of these  elements are to be displayed.
## A CSS rule contains two elements a (Selector, and a declaration) 
###  Selectors indicate which element the rule applies to
### Declarations indicate how the elements reffered to in the selector should be styled.

### CSS declarations sit inside curly brackets and each is made up of two parts (Property and Value) which is separated by a colon.

* `<link>` Can be used in a HTML document to tell the browser where to find a CSS file, and does not need a closing tag which is important to keep in mind.  It has the three attributes listed below
* `<href>` Specifies the path to the CSS file
* `<rel>` Specifies the relationship with the HTML page and the file it is connecting to (ex. stylesheet when connecting to CSS)
* `<type>` Specifies type of document such as txt/css

## Placing CSS directly into the HTML file
* `<style>` Usually placed within the `<head>` tag 
* The `<style>` element should indicate the type attribute in order to specify CSS or whatever the type may be 

### When building a site with more than one page an external style sheet should be used

# CSS selectors

There are various selectors so i'll cover a few below

* `* {}` Targets all elements on a page
* `.name{}` Targets the Element whos class attribute who has a value of name
* `#name{}` Targets the Element whos id attribute who has a value of name

# Selectors

### If the two selectors are identical the latter of the two will take precedence
### Specificity - if one selector is more specific than the other the one that is more specific will take precedence over the others 
### `!important` can be added after any property value to indicate it should be considered more important to any other rules that apply to the same element

# Inheritance 

### Inheritance is important because if you were to change something with the `<body>` element it would affect each child element of that body tag since child elements inherit the parent elements changes.

# Javascript

## A script is a series of instructions that a computer can follow one by one.  Each invdividual steps or instructions is known as a statement.  Statements need to end with a semicolon (;)

### Javascript 

* Java script is case sensitive
* Statements are instructions that the computer should follow and each one starts ona new line (Helps with code clarity)
* Statements can be organized into code blocks (The curly braces are not followed by a semi colon)
* Comments should be utilized in order to explain what the code does
* There are block comments and single line comments to be utilized in javascript
* When a script needs to temporarily store its bits of information necessary to do its job it uses a (Variable)
* A variable has a perfect name for what it does in the sense that it can chang according to the data stored in it (vary)
* To declare a variable we must first use (var) followed by the variable name and then a semicolon;
* Javascript Interpreter knows that var is a keyword 
* Each variable needs to be assigned a name or identifier 
* Variable names with more than one word uses camelCase
* Assignment operator is an equal sign
* Numeric data handles numbers
* The strings data type is put within quotations 
* Boolean data type is (True or False)
* Arrays (Special type of variable) - However instead of jus storing one value it stores a list of values.
* Important to note that the values of an array start with a 0 and not a 1
* Each item in an array is automatically given a number called an index
* Expressions rely on operators

# Operators

* Assignment operator
* Arithmetic operator
* String operator
* Comparison operator
* Logical operator

# Decisions and loops

* There are several places within a script where decisions need to be made and flowcharts can help make these decisions.

## There are two components to a decision:
### 1) An expression is evaluated, which returns a value 
### 2) A conditional statement says what to do in a given situation


# Comparison operators: evaluating conditions 
* `==` is equal to
* `!=` is not equal to
* `===` Strictly equal to
* `!==` Strictly not equal to
* `>` Greater than
* `<` Less than
* `>=` Greater than or equal to
* `<=` Less than or equal to

## In any condition there is one operator and two operands

# Logical Operators

* && Logical and
* || Logical or
* ! Logical not

# Statements

* IF statements evaluates or checks a condition.
* IF - ELSE  statements checks a condition

# Switch Statements

> A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value.

* If the switch value does not match any of the values within its brackets then the default value is given.
* Instead of multiple if statements, the code is ran if a match is found.  And there is always a default to fall back on


