# Error Handling & Debugging

* The Console & Dev Tools - Tools build into the browser that help you hunt for errors
* Common Problems - Common sources of errors and best practices to solve them
* Handling Errors - How code can deal with potential errors gracefully

-Order of Execution
*Knowing how scripts are processed can help one to find an error.

> The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope.

-Global context - Code that is in the script, but not in a function. There is only one global context in any page.
-Global scope - If a variable is declared outside a function, it can be used anywhere because it has global scope.  If the (VAR) Keyword is not used when creating a variable, it is placed in the global scope.
-If a variable is declared within a function it can only be used within that function (This is due to it having function-level scope).

> The javascript interpreter processes one line of code at a time. When a statement needs data from another function, it stacks (or piles) the new function on top of the current task.


> Each time a script enters a new execution context, there are two phases of activity:

-Prepare
-Execute

## Scope

-Located in the interpreter every execution context has its own variables object.
Holding variables, functions, and parameters allocated to it.
Every execution context can access it's parent's variables object.

-Javascript have lexical scope - they are linked to the object they were defined within

-Children can ask the parents for variable information but parents cannot ask children

-Syntax error (Reference Error)
-Reference error (Variable does not exist)
-Error
-TypeError
-RangeError
-URI Error
-EvalError

### How to deal with errors

-Debug the script to fix errors
-Handle errors gracefully

* Utilize a debugging workflow

-Where is the problem?
-What exactly is the problem


### Chrome developer tools

-The line number of the error does not always show exactly where the error is, but instead it is where the interpreter noticed there was a problem with the code

> Browsers that have a console have a console object, which has several methods that your script can use to display data in the console. The object is documented in the Console API.

-Chrome gives a detailed description of this API on it's website and how a developer can best utilize it

`console.log()`

> The console.log() method can write data from a script to the console. If you open console- l og. html, you will see that a note is written to the console when the page loads.
> Such notes can tell you how far a script has run and what values it has received. In this example, the blur event causes the value entered into a text input to be logged in the console.
> Writing out variables lets you see what values the interpreter holds for them. In this example, the console will write out the values of each variable when the form is submitted.

- the `console.log()` method can write several values to the console at the same time

* More console methods

-`console.info()`
-`console.warn()`
-`console.error()`
-`console.group()`
-`console.assert()`

> You can pause the execution of a script on any line using breakpoints. Then you can check the values stored in variables at that point in time.

# Breakpoints can help narrow down a problem 

-If you set multiple breakpoints you can walk through them one by one in order to see where values are being changed and where the problem could possibly occur

> If you know your code might fail, use try, catch, and finally. Each one is given its own code block.
-Try 
-Catch
-Finally

> If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them.

* `throw new Error( 1message 1) ;`

# Debugging tips

-Utilize a second browser
-Search
-Validation Tools
-Add numbers
-Strip it back
-Code playgrounds
-Explaining the code

## Go over common errors

- Mixed/Extra Characters
- Data Type Issues
