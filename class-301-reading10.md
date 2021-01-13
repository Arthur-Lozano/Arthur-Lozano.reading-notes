# Types of error messages

- Reference errors
- Syntax errors
- Range errors
- Type errors

## Debugging

> To debug your JS code, the easiest and maybe the most common way its to simply console.log() the variables you want to check or, by using chrome developer tools, open your page with your JS code (press cmd+o in macOS or Ctrl+o in Windows) and choose your file to debug, click the line you wanna debug and refresh your page again (F5).

## CallStack

> The JavaScript engine (which is found in a hosting environment like the browser), is a single-threaded interpreter comprising of a heap and a single call stack. The browser provides web APIs like the DOM, AJAX, and Timers.

- The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.
- The understanding of the call stack is vital to Asynchronous programming
- In Asynchronous JavaScript, we have a callback function, an event loop, and a task queue. The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop.

* At the most basic level, a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

- The red part of our first example represents the call stack, which is the path that your program has taken to reach the point were you set a breaking point or were you have an error.

> A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

>When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.  Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.  When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.  If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.

Reference: https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/
Reference:https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7
Reference:https://developer.mozilla.org/en-US/docs/Glossary/Call_stack