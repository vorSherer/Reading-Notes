# Read 04 - Classes, Objects and Recursion in Python

#### 2020-06-09

## RESOURCES:
#### Classes and Objects <br>
https://www.learnpython.org/en/Classes_and_Objects <br>
#### Thinking Recursively (Optional: 'Naive Recursion is Naive' section and beyond) <br>
https://realpython.com/python-thinking-recursively/ <br>
#### Pytest Fixtures and Coverage <br>
https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage <br>
#### Pytest Fixtures <br>
https://docs.pytest.org/en/latest/fixture.html <br>

## Classes and Objects <br>
"Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects." <br>
A Class may be treated as a template for data, similar to a Constructor in JavaScript. A Class may be defined, containing variables, functions, etc. (e.g., "class MyClass:" with it's contents). One or more variables ("object instances") may be assigned a class (e.g., "myobjecta = MyClass"), which brings in all the functionality of MyClass, but the values of which may be customized to the object instance (e.g., "myobjecta.variable = 'New value'").

## Thinking Recursively (Optional: 'Naive Recursion is Naive' section and beyond) <br>
#### Recursive Functions in Python
__The formal definition of a recursive function__ is, *"A recursive function is a function defined in terms of itself via self-referential expressions."* This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result. <br>
__All recursive functions share a common structure made up of two parts: *base case* and *recursive case*.__ <br>
As the large problem is broken down into successively less complex ones, those subproblems must eventually become so simple that they can be solved without further subdivision. This is the __*base case*__. <br>
#### Maintaining State 
Each recursive function call has its own execution context, so to maintain state during recursion you have to either: <br>
* Thread the state through each recursive call so that the current state is part of the current call’s execution context (i.e. passing the updated current state to each recursive call as arguments), or <br>
* Keep the state in global scope (resulting in mutable global state - not very pythonic!).
#### Naive Recursion is Naive 
Naively following the recursive deﬁnition of say, the nth Fibonacci number, is rather inefficient; doing so results in unnecessarily recomputing values.  At scale, this can seriously degrade performance and unnecessarily consume resources. Caching results for reuse is an effective way to avoid this (see [Python + Memcached: Efficient Caching in Distributed Applications](https://realpython.com/python-memcache-efficient-caching/) for further explanation). <br>

## Pytest Fixtures and Coverage <br>
Additional background material at [Testing Your Code with Python's pytest](https://www.linuxjournal.com/content/testing-your-code-pythons-pytest) and [Testing Your Code with Python's pytest, Part II](https://www.linuxjournal.com/content/testing-your-code-pythons-pytest-part-ii). <br>
Two features built into pytest are __*Fixtures*__ and __*Code Coverage*__. <br>
#### Fixtures 
When you're writing tests, in many cases, you'll have a few tests with similar characteristics, something that pytest handles with __*"parametrized tests"*__. <br>
If you want some objects available to all of your tests, perhaps because they contain data you want to share across tests, or they might involve the network or filesystem. These are often known as "fixtures" in the testing world. In pytest, you define fixtures using a combination of the __*pytest.fixture*__ decorator, along with a *function definition*. <br>
#### Coverage 
"Code coverage" refers to checking that your tests have run all of the code - harder to verify when code bases get large and complex. <br>
Pytest includes a package called __*pytest-cov*__ on PyPI that you can download and install. Once that's done, you can invoke pytest with the __*--cov*__ option (provide an argument to --cov, specifying which program(s) you want to test - e.g., "pytest --cov=mymul ."). Also indicate the directory into which the report should be written and turn the coverage report into something human-readable (e.g., "coverage html").

## Pytest Fixtures
Pytest has useful built-in fixtures. Fixtures are defined using the __*@pytest.fixture*__ decorator after adding "import pytest" to your test file. <br>
Test functions can receive fixture objects by naming them as an input argument. For each argument name, a fixture function with that name provides the fixture object. Fixture functions are registered by marking them with __@pytest.fixture__. <br>
Fixtures allow test functions to easily receive and work against specific pre-initialized application objects without having to care about import/setup/cleanup details. It’s a prime example of dependency injection where fixture functions take the role of the injector and test functions are the consumers of fixture objects.
#### Fixture finalization / executing teardown code 
Pytest supports execution of fixture-specific finalization code when the fixture goes out of scope. By using a __*yield*__ statement instead of __*return*__, all the code after the yield statement serves as the *teardown code*.
