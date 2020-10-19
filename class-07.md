
# DOM Modeling

> Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model

## Define a constructor and initialize properties
- define the same properties between many objects, we need to use a constructor function

- The constructor function is defined using a function expression
- A variable is define and assigned a function with parameters
- When the function is called, the data inside the parameters are stored inside the this.parameter and this.parameter properties. Storing data within properties ensures any *newly created object can access that data later.

* When an object is instantiated you are creating in instance of that object, using the (new) keyword.

* after being instatiated and initialized these objects are stored inside their variables

> This is object-oriented programming in JavaScript at its most fundamental level.
> The new keyword instantiates (i.e. creates) an object.
The constructor function initializes properties inside that object using the this variable.
The object is stored in a variable for later use.

> This is object-oriented programming in JavaScript at its most fundamental level.

The new keyword instantiates (i.e. creates) an object.
The constructor function initializes properties inside that object using the this variable.
The object is stored in a variable for later use.

> As you can see, methods can be added to a constructor function's prototype. Think of the prototype as an object's stunt double. Whenever a scene is too dangerous, you can substitute in the prototype to do the work while the object takes all the glory

### Important
> And shared code means a running program consumes less memory which is important for devices like smart phones and tablets.

# Chapter 6: “Tables” (pp.126-145)

## Basic Table Structure

- `<table>`
- `<tr>`
- `<td>`
## Table Headings

- `<th>`

## Spanning Columns

> The colspan attribute can be used on a `<th>` or `<td>` element and indicates how many columns that cell should run across.
## Spanning Rows

> The rowspan attribute can be used on a <th> or <td> element to indicate how many rows a cell should span down the table.

## Long Tables

> There are three elements that help distinguish between the main content of the table and the first and last rows (which can contain different content).
- `<thead>`
- `<tbody>`
- `<tfoot>`

* width and spacing can be declared with the table tag or css
* Border & Background - The border attribute was used
on both the `<table>` and `<td>`
elements to indicate the width of
the border in pixels.

# Chapter 3: “Functions, Methods, and Objects” (pp.106-144)

### Creating an object: constructor notation

- The (new) keyword and the object constructor create a blank document.  You can then add properties and methods to the object.

* First create a new object using a combination of (new) keyword and the `Object()` constructor function. 
- After creating a blank object you can add properties and methods to it using (dot notation).
- Every statement that adds a property or method should end with a semicolon.
-to create an empty object using literal notation `var objectName = {}`

### Updating an object

- To update the value of properties use dot notation or square brackets.  They work on objects that were created using literal or constructor notation.  If you want to delete a property use the (delete) keyword.

- You can update properties of an object but not the method using square bracket syntax. Object name followed by square brackets, and the property name belongs inside the square brackets for example `room['small']='park';`

- In order to clear the value of a property it needs to be set to a blank string like this `room.name = ''`;

### Creating many objects using constructor notation

- Used if you want many objects to represent similar things.
- Object constructors can use a function as a template for creating objects.

* The first step is to create the template with the object's properties and methods.

* The name of a constructor function usually begins with a capital letter (which usually begin with a lowercase character)

# New keyword reminder
* The uppercase letter is supposed to help remind developers to use the `NEW` keyword when they create an object using that function.

- The new keyword followed by a call to the function creates a new object.
* The properties of each object are given as arguments to the function.

- to delete a property, use the keyword delete.(property or method)

- The (this) keyword always refers to one object, usually the object in which the function operates.

- Arrays are objects

- Arrays and objects can be combined in order to create complex data structures.  Arrays can store objects and objects can also hold arrays (as values of their properties)

> The DOM is vital to accessing and amending the contents of the current web page.



