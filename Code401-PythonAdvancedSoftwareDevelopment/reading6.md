# Reading 4

## How to use Random python modules

> The random module provides access to functions that support many operations. Perhaps the most important thing is that it allows you to generate random numbers.

example:
* import random
* random.random() * 100
### methods
- Random - give random number
- Choice - The choice function can often be used for choosing a random element from a list.
- Shuffle - The shuffle function, shuffles the elements in list in place, so they are in a random order.
- RandRange - Generate a randomly selected element from range(start, stop, step)

### What is Risk Analysis in Software Testing and how to perform it?

> The probability of any unwanted incident is defined as Risk. In Software Testing, risk analysis is the process of identifying the risks in applications or software that you built and prioritizing them to test. After that, the process of assigning the level of risk is done. The categorization of the risks takes place, hence, the impact of the risk is calculated.

- Why use Risk Analysis?
* Risk analysis helps to identify potential problem areas or situations we woud like our software from being exposed to.  After finding out these problem areas we could incorporate them into our tests in order to try to mitigate them or avoid them all together.

### example risks:
- Use of new hardware
- Use of new technology
- Use of new automation tool
- The sequence of code
- Availability of test resources for the application

- Risk Identification

* Business Risks: This risk is the most common risk associated with our topic. It is the risk that may come from your company or your customer, not from your project.

* Testing Risks: You should be well acquainted with the platform you are working on, along with the software testing tools being used.

* Premature Release Risk: a fair amount of knowledge to analyze the risk associated with releasing unsatisfactory or untested software is required

* Software Risks: You should be well versed with the risks associated with the software development process.

- Risk Assessment

* Early forecast of unwanted situations in your project

* Estimating potential loss of such situations

* Making decisions to deal

* Avoid the future consequences

- Perspective of Risk Assessment

* Effect

* Cause

* Likelihood

- How to perform Risk Analysis?

* Searching the risk

* Analyzing the impact of each individual risk

* Measures for the risk identified

- TestCoverage
> Test coverage is a useful tool for finding untested parts of a codebase. Test coverage is of little use as a numeric statement of how good your tests are.
- But even without that you get lots of tests looking for things that rarely go wrong distracting you from testing the things that really matter.
- A coverage percentage of 80 or 90% would be expected, a coverage percentage of 100 might raise questions as to if someone is writing the tests just to pass.
- One sign you are testing too much is if your tests are slowing you down. If it seems like a simple change to code causes excessively long changes to tests, that's a sign that there's a problem with the tests.







### References
- https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python
- https://martinfowler.com/bliki/TestCoverage.html
- https://www.edureka.co/blog/risk-analysis-in-software-testing/