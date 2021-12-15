# Reading 4

## Classes and Objects

> Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.

- Create the class which when instantiated will create new objects that inherit the same traits as the base class (variables and functions)

- Accessomg a variable in a class can be done with dot notation.

> init() - The __init__() function, is a special function that is called when the class is being initiated. It's used for asigning values in a class.
> class NumberHolder:
   def __init__(self, number):
       self.number = number

## Thinking Recursively

- Optional: Naive Recursion is Naive section and beyond

> Typical structure of a recursive algorithm. If the current problem represents a simple case, solve it. If not, divide it into subproblems and apply the same strategy to them (recursion)

- A recursive function is a function defined in terms of itself via self-referential expressions.

- All recursive functions share a common structure made up of two parts: base case and recursive case.

- When dealing with recursive functions, keep in mind that each recursive call has its own execution context, so to maintain state during recursion you have to either:  Thread the state through each recursive call so that the current state is part of the current call’s execution context
Keep the state in global scope

## Pytest Fixtures and Coverage

- fixtures 
* In pytest, you define fixtures using a combination of the pytest.fixture decorator, along with a function definition.
* Instead of defining global variables in your test file, you can create a fixture that'll provide your test with the appropriate object at the right time.

- code coverage - checking that our test has covered all code.
* --cov, specifying which program(s) you want to test. And, you should indicate the directory into which the report should be written. So in this case, you would say:

### References
- https://www.learnpython.org/en/Classes_and_Objects
- https://realpython.com/python-thinking-recursively/
- https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage