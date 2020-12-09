# Read: 02 - jQuery, Events, and The DOM

- jQuery lets you find elements using css-style selectors and then munipulate the elements using jquery methods.
- the jQuery() function allows you to find one or more elements within the page and has been shortened to $().
- the jQuery object has plenty of methods that can be used to work with the element you select.
- the (.) = member operator - indicated the method on the right should be used to update the element on the left (within the jquery Object).
- The parameters of the method provide details about how to update the element, this parameter specifies a value to add to the class attribute.
- Event handing is simpler since it uses one method that works across all major browsers.
- jQuery doesn't do anything that cannot be done with pure Javascript but is used because it makes coding easier
- jQuery uses CSS selectors to select elements
* jQuery has methods that offer web developers simpler ways to perform common tasks, for instance:
- Loop through elements
- Add/remove elements from the DOM tree
- Handle events
- Fade elements into/out of view
- Handle Ajax requests
### jQuery's motto is "Write less, do more," because it allows ou to achieve the same goals but in fewer lines of code than you would need to write with plain javascript.

- When you select one or more elements a jQuery object is returned, also known as a "matched set" or a jquery selection.
- An example would be ul and li nodes
- Each element is given an index number starting with 0
- If a jQuery selection holds more than one element, and a method is used to get information from the selected element it will only retrieve information from the the (first element) in the matched set.
- Utilizing the li element as before would only retrieve informaiton from the first li element as opposed to all elements; however, there are various methods to traverse through elements
- To get the content of all of the elements `.each()` method should be looked at.
* Set Information
- If a jQuery selection holds more than one element and a method is used to update information on a page it will update (ALL OF THE ELEMENTS) in the matched set, not just the first one.
- So unlike getting information in jQuery where you only get the first element, setting information will set all the elements
- There are also methods to traverse the DOM to choose specific elements to update
* Jquery objects store references to elements
> When you create a selection with jQuery, it stores a reference to the corresponding noes in the DOM tree.  It does not create copies of them.
- When you create a jQuery selection, the (jQuery object holds references to the elements in the DOM)
- A variable or object is sotring a reference to something, what it is doing is storing the location a piece of information in the browser's memory.  
> The jQuery object is an array-ike object becausei t stores a list of elements in the same order that they appear in the HTML document.
- This is unlike other objects where the order of each property is preserved.
- A jQuery object stores references to elements.  
* Caching a jQuery object stores a reference to it in a variable.

* Creating a jQuery Object
- Find matching nodes in the DOM tree
- Create the jQuery object
- Store references to the nodes in the jQuery object
- jQuery objects are often given a name beginning with $
- jQuery can update all elements with out a loop

*Implicit iteration
- The ability to update all of the elements in the jQuery selection is known as implicit iteration
- When it is needed to get information from a series of elements, `.each()` method can be used.

### Chaining
- Using more than one jQuery method on the same selection of elements you can list several methods at a time using dot notation to seperate each method.
- CHAINING is the process of placing several methods in the same seleector. (Providing more compact and cleaner code)
* Most methods used to UPDATE the jQuery methods can be chained.
* Most methods used to RETRIEVE  information from the DOM CANNOT be chained.
- Also, if one of the methods in the chain does not work most likely the rest of the methods will not work either.

- .reaad() method checks that the page is ready for the code to work with
- (document) creates a jQuery object representing the page and then when the page is ready the function that is placed within the parentheses runs.

- `.on()`
- `.ready()`
- Place scripts before closing body tags

* Positive side-effect of writing jQuery code inside the method is that it creates function-level scope for its variables.

- Any statments inside the method automatically run when the page is loaded.

- .html and .text methods both retrieve and update the content of elements.
- .html - only retrieves HTML inside the first element in the matched set along with it's descendents.  If anything else needs to be retrieved look at .each.
- .text - returns content from every element in the jQuery selection along with the text from any descendants.  Also returns spaces between words.  To get content from 'input' or 'textarea' elements use the .val method.

* Four methods for updated content on all elements in a jQuery selection
- .html() - This method gives every element
in the matched set the same new
content. The new content may
include HTML.
- .text() This method gives every element
in the matched set the same new
text content. Any markup would
be shown as text.
- .replaceWith()
- .remove() - This method replaces every
element in a matched set with
new content. It also returns the
replaced elements.

- When updating the content of an element you can use a string, a variable and or a function.

### Inserting new elements involves 2 Steps
- 1. Create the new elements in a jQuery object
- 2. Use a method to insert the content into the page
* Methods to add content to the DOM tree

- .before() This method inserts content
before the selected element(s) 
- . after() This method inserts content
after the selected element (s)
- .prepend() - This method inserts content
inside the selected element(s),
after the opening tag
- .append() - This method inserts content
inside the selected element(s),
before the closing tag
- . prependTo()
- . appendTo()

## You can create attributes, or access and update their contents, using the following four methods.

-.attr()
-.removeAttr()
- .addClass()
-.removeClass()

## GETTING & SETTING CSS PROPERTIES

- The . css () method lets you retrieve and set the values of CSS properties.

- CSS property and it's value are seperated by a comma instead of a colon
> When dealing with dimensions that are specified in pixels. you can increase and decrease the va lues using the+= and-= operators. ${'li ' ).css( 'padding-left', '+=20' )

### You can set multiple properties using object literal notation:

* Properties and values are placed in curly braces
* A colon is used to separate property names from their values
* A comma separates each pair (but there is not one after the last pair)This sets the background color and typeface for all list items.

- jQuery allows you to recreate the functionality
of a loop on a selection of elements, using the each () method.

- Why a loop might be necessary 
* Get information from each
element in the matched set.
* Perform a series of actions on
each of the elements.

### This is why the .each() method is provided.
- The parameter of the .each() method is a function
- This could be an anonymous function or a named function
> • each() Allows you to perform one or more statements on each of the items in the selection of elements that is returned by a selector - rather like a loop in JavaScript. It takes one parameter: a function containing the statements you want to run on each element.

> this or $(this) As the . each() method goes through the elements in a selection, you can access the current element using the this keyword.You also often see $ (thi s), which uses the this keyword to create a new jQuery selection containing the current element. It allows you to use jQuery methods on the current element.
- $(this) is used to create a jQuery object that contains the current element in the loop.
- after having the current element other methods can be used on it

## EVENT METHODS

- .on() method is used to handle all events
- jQuery handles all cross-browser issues
- use a selector to create a jQuery selection
> Use .on() to indicate which event you want to respond to. It adds an event listener to each element in the selection.
- The . on() method is used to handle events. It needs two parameters:
* The first parameter is the event you want to respond to
* The second parameter is the code you want to run when that event occurs on any element in the matched set, could be a named function or anonymous function

- jQuery events
* UI - focus , blur, change
* KEYBOARD - input, keydown, keyup, keypress MOUSE
* Mouse - click, dblclick, mouseup, mousedown,mouseover, mousemove,mouseout, hover*
* Form - submit, select, change
* DOCUMENT -ready* , load, unload*
* BROWSER error, resize , scro11

## THE EVENT OBJECT

> Every event handling function receives an event object. It has methods and properties related to the event that occurred.

* 1. Give the event object a parameter name.
* 2. Use that name in the function to reference the event object.
* 3. Access the properties and methods of the object using the familiar
dot notation (the member operator).

# 6 Reasons for Pair Programming
- Greater efficiency - easy to catch mistakes and derive ideas.
- Engaged Collaboration - Easier to stay on track and focused on the task when working with a partner.  No more than 15 minutes should pass by before seeking help.
- Learning from fellow students - Working with teammates can help individuals get out of their shell and try working on projects form a different approach they might not have otherwise have attempted.
- Social Skills - This can foster growth with working with other people.  This isn't just a school benefit but also when working for an employer.  Being able to learn to communicate well and convey what needs to be said in order to get a task accomplished can go a long way.
- Job interview readines - Building on job interview readiness is key, being able to code with a potential employer or answer questions to solving problems via code challenges is a skill that must be built on and mastered as much as possible to prepare for the future.
- Work environment readiness - Code fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.

