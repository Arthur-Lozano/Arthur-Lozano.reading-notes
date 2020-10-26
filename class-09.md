# Forms
### Forms allow a user to have various control within or on a website
- Input
- Adding text
- Making Choices
- Submitting Forms
- Uploading Forms

## Form Structure

`<form>`
> This element should always carry the action attribute and will usually have a method and id attribute too.
> action Every `<form>` element requires an action attribute. Its value is the URL for the page on the server that will receive the information in the form when it is submitted.
- `action`
- `method` Either get or post

## Text Input

- `<textarea>`
- `<input>` Is used to put user input into the form
- type = text 
- type = password
- type = radio
- type - checkbox
- type = date
- type = email
- type = url
- type = search

## Drop down List

- `<select>`
- `<option>`
* size
* multiple

- Submit Button
- Image Button
- Button and Hidden Controls
- Labeling Form Controls
- Grouping Form Elements
* `<fieldset>`
- Group related form controls
* `<legend>`
- Helps identify the purpose of the group of form controls
* Form validation
- Used to display a message if the form isn't entered correctly

* Placeholder
- Used to hold text before a user enters data into a text box

# Lists Tables and Forms

### List style type
- UL
- OL

* Table properties 

- width
- padding
- text-transform
- letter-spacing, font-size
- border-top, border-bottom
- text-align
- background-color
- :hover
- Cell padding - keep text away from touching a table
- Distinguish heading `<th>`
- Shade alternate rows
- Align numerals
- Online Extra

* Border on empty cells
- Show
- Hide
- Inherit

* Gaps between cells
- Collapse
- Separate

* Styling text inputs
- font-size
- color (sets text color)
- background-color (sets backgrounds color)
- border (sets border around input box)
- border-radius (can be used to create rounded corners)
> The :focus pseudo-class is used to change the background color of the text input when it is being used, and the :hover psuedo-class applies the same styles when the user hovers over them.
- background - image

* Styling Fieldsets & Legends 
- width
- color
- background-color
- border
- border-radius 
- padding (used to add spacing inside these elements)
- 

# Events


* UI events
- load
- unload
- error
- resize
- scroll
* Keyboard events
- keydown 
- keyup
- keypress
* Mouse Events
- click
- dbclick
- mousedown
- mouseup
- mousemove
- mouseover
- mouseout


* Other 

- Fired or Raised = Code is triggered
> When an event has occurred, it is often described as having fired or

> EVENTS TRIGGER SCRIPTS Events are said to t rigger a function or script. When the click event fires on the element in this diagram, it could trigger a script that enlarges the selected item. been raised. In the diagram on the right, if the user is tapping on a link, a click event would fire in the browser.
- Event types:
* click
* mouseover
* submit
* page load

# Event Listeners

- Code that is going to trigger when event is fired

- Bind: bind or tether an event listener to the event

- Event capturing

- Event Bubbling


# Various

> When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code. Together these steps are known as event handling.
- 1. Select the element nodees you want the script to respond to
- 2. Indicate which events on the selected nodes will trigger a response (Binding the event to the DOM)
- 3. State the code you want to run when the event occurs

## There are three types of event handlers

- HTML Event Handlers
- Traditional DOM event handlers
- DOM Level 2 event handlers

* Traditional DOM event handlers
- You can only attach one function to each event handler

> can only attach one function to each event handler. Here is the syntax to bind an event to an element using an event handler, and to indicate which function should execute when that event fires:
- `element.oneevent = functionName;
-  Element-Event -     code

### Event listers are more efficient than the older DOM event handlers

> Event listeners are a more recent approach to handling events. They can deal with more than one function at a time but they are not supported in older browsers.

* Event bubbling - Event starts at the most specific node and flows out to the last specific node

- The flow of events only really matters when your code has event handlers on an element and one of it's ancestors or descendent elements.

* The Event Object 
- When an event occurs, the event object tells
you information about the event, and the
element it happened upon.

* Using event listeners withe the event object

> Creating event listeners for a lot of elements can slow down a page, but event flow allows you to listen for an event on a parent element.

> The event object has methods that change: the default behavior of an element and how the element's ancestors respond to the event.

- preventDefault ()
- stopPropagation()
- USING BOTH METHODS

* MUTATION EVENTS & OBSERVERS

- Whenever elements are added to or removed from the DOM, its
structure changes. This change triggers a mutation event.

* HTM LS EVENTS

- DOMContentLoaded
- hashchange
- beforeun load
