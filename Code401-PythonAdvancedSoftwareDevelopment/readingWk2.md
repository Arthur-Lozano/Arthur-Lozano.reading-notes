# Reading Week 2

## In tests we trust

> Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.

- TDD on the otherhand is to write tests first.

## If name equals main

> Before executing code, Python interpreter reads source file and define few special variables/global variables. 
If the python interpreter is running that module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable. 

- Thus, you can test whether your script is being run directly or being imported by something else by testing __name__ variable.
If script is getting imported by some other module at that time __name__ will be module name.

- Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.
If you import this script as a module in another script, the __name__ is set to the name of the script/module.
Python files can act as either reusable modules, or as standalone programs.
if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported.


## Recursion

* The process of a function calling itself directly or indirectly.

### References
- https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932
- https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/
- https://www.geeksforgeeks.org/recursion/