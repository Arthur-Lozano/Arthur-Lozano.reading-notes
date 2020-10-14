# Problem Domain, Objects, and the DOM

## Chapter 3: “Object Literals” (pp.100-105)

* Objects group together a set of variables and functions in order to create to create a model of something that you would recognize in the real world. Within an object variables and functions take on new names.
* Within an object variables become known as properties (properties tell us about an object/describe the object)

### In an object functions become known as methods
* If a function is part of an object , it is called a method.

* If a variable is part of an object it is called a property.

## Creating an object

- Literal notation is the easiest and most popular way to crete objects (There are more than one option when creating options)

- The object is within curly brackets that are normally stored within a variable name and you can refer to it by that variable name.

* Separate each property and method with a comma.
* Separate each key from it's value with a colon.

> You access the properties or methods of an object using dot notation.  You can also access properties using square brackets.
> To access a property or method of an object you use the name of the object, followed by a period, then the name of the property or method you want to access. This is known as dot notation.

- The period is known as the member operator. The property or method to the right is a member of the object on the left.
- Properties of an object can also be accessed using square brackets (but not the method)

> Similarly, to use the method, you can use the object name followed by the method name. hotel .checkAvailability()
>If the method needs parameters, you can supply them in the parentheses (just like you can pass arguments to a function).
> If you had two objects on the same page, you would create each one using the same notation but store them in variables with different names.


## Chapter 5: “Document Object Model” (DOM) (pp.183-242)

### 

> The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

> The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules. It is implemented by all major browser makers, and covers two primary areas:
- MAKING A MODEL OF THE HTML PAGE
> You will hear people call the DOM an Application Programming Interface (API). User interfaces let humans interact with programs; APls let programs (and scripts) talk to each other. The DOM states what your script can "ask the browser about the current page, and how to tell the browser to update what is being shown to the user.

- ACCESSING AND CHANGING THE HTML PAGE

> The DOM specifies the way in which the browser should structure this model using a DOM tree. The DOM is called an object model because the model (the DOM tree) is made of objects. Each object represents a different part of the page loaded in the browser window.

-  The DOM tree is a model of the web page
- Above, you can see the HTML code for a shopping
list, and on the right hand page is its DOM tree.
Every element, attribute, and piece of text in the
HTML is represented by its own DOM node.
- To access the DOM tree, you start by looking for
elements. Once you find the element you want, then
you can access its text and attribute nodes if you
want to.
- Each node is an object with methods and properties.

> Scripts access and update this DOM tree (not the source HTML file). Any changes made to the DOM tree are reflected in the browser.

> TEXT NODES Once you have accessed an element node, you can then reach the text within that element. This is stored in its own text node. Text nodes cannot have children. If an element contains text and another child element, the child element is not a child of the text node but rather a child of the containing element. (See the `<em>` element on the first `<li >` item.) This illustrates how the text node is always a new branch of the DOM tree, and no further branches come off of it.

> ATTRIBUTE NODES
> The opening tags of HTML elements can carry attributes and these are represented by attribute nodes in the DOM tree.

## SELECT AN INDIVIDUAL ELEMENT NODE

- getElementByld ()
- querySe1ector ()

## SELECT MULTIPLE ELEMENTS (NODELISTS)

- getElementsByClassName()
- getElementsByTagName()
- querySelectorAll()

## TRAVERSING BETWEEN ELEMENT NODES

- parentNode
- previousSibling / nextSibling
- firstChild / lastChild

> FASTEST ROUTE - Finding the quickest way to access an element within your web page will make the page seem faster and/or more responsive. This usually means evaluating the minimum number of nodes on the way to the element you want to work with. For example, getEl elementByld() will quickly return one element