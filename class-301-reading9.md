# Read: 09 - Refactoring

* Concepts of Functional Programming in Javascript

> Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 

* pure functions
- It returns the same result if given the same arguments (it is also referred as deterministic)
- It does not cause any observable side effects
- If our function reads external files, it’s not a pure function — the file’s contents can change.
- Any function that relies on a random number generator cannot be pure.
* Examples of observable side effects include modifying a global object or a parameter passed by reference.

## Pure functions benefits

- The code’s definitely easier to test. We don’t need to mock anything. * So we can unit test pure functions with different contexts:
* Given a parameter A → expect the function to return value B
* Given a parameter C → expect the function to return value D

## Immutability

* Unchanging over time or unable to be changed.
* When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.
- But how do we handle mutability in iteration? > Recursion!
> Recursion is a technique for iterating over an operation by having a function call itself repeatedly until it arrives at a result. Most loops can be rewritten in a recursive style, and in some functional languages this approach to looping is the default.

> One reason that recursion is favored in functional programming languages is that it allows for the construction of code that doesn’t require setting and maintaining state with local variables. Recursive functions are also naturally easy to test because they are easy to write in a pure manner, with a specific and consistent return value for any given input, and no side effects on external variable states.

- With recursion, we keep our variables immutable

- Basically, if a function consistently yields the same result for the same input, it is referentially transparent.

* `pure functions + immutable data = referential transparency`.

- The idea of functions as first-class entities is that functions are also treated as values and used as data.
Functions as first-class entities can:
refer to it from constants and variables
pass it as a parameter to other functions
return it as result from other functions

- The idea is to treat functions as values and pass functions like data. This way we can combine different functions to create new functions with new behavior.

# Refactoring JavaScript for Performance and Readability

> It's important to get your code right the first time because in many businesses there isn't much value in refactoring. Or at least, it's hard to convince stakeholders that eventually uncared for codebases will grind productivity to a halt.





Reference: https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec
Reference:https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa