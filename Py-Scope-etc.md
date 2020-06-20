# Read 07 - Python Scope and misc

#### 2020-06-20

## RESOURCES:
#### Python Scope (global and nonlocal keywords) <br>
https://realpython.com/python-scope-legb-rule/ <br>
#### Don’t be CONFUSED by BIG O notation anymore! <br>
https://www.youtube.com/watch?v=5Uqawfl0VHQ <br>
#### Rolling Dice Examples  <br>
https://artofproblemsolving.com/wiki/index.php/Basic_Programming_With_Python#Program_Example_1_3 <br>


#### Python Scope (global and nonlocal keywords) <br>
This thorough article includes a descriptive comparison of Local, Enclosing, Global and Built-in scope (collectively referred to as the LEGB rule, after the order in which python looks up a name. If it can’t find the name, then you’ll get an error.). <br>
Throughout the article, the term __*'name'*__ refers to the identifiers of variables, constants, functions, classes, or any other object that can be assigned a name. The names in one's programs will have the scope of the block of code in which one defines them. Thus the names that one defines in __Global__ scope are available to all one's code. <br>
__Enclosing (or nonlocal)__ scope is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function. This scope contains the names that you define in the enclosing function. The names in the enclosing scope are visible from the code of the inner and enclosing functions. <br>

"By default, parameters and names that you assign inside a function exist only within the function or local scope associated with the function call. When the function returns, the local scope is destroyed and the names are forgotten. Here’s how this works: <br>

<pre><code>>>> def square(base):
...     result = base **
...     print(f'The square of {base} is: {result}')
...
>>> square(10)
The square of 10 is: 100
>>> result  # Isn't accessible from outside square()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
    result
NameError: name 'result' is not defined
>>> base  # Isn't accessible from outside square()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
    base
NameError: name 'base' is not defined
>>> square(20)
The square of 20 is: 400</code></pre> <br>

__square()__ is a function that computes the square of a given number, base. When you call the function, Python creates a local scope containing the names __base__ (an argument) and __result__ (a local variable). After the first call to *square()*, *base* holds a value of 10 and *result* holds a value of 100. The second time, the local names will not remember the values that were stored in them the first time the function was called. Notice that *base* now holds the value 20 and *result* holds 400." <br>

#### Don’t be CONFUSED by BIG O notation anymore! <br>
This YouTube video seeks to offer yet another simplified explanation of what Big O is and how it works. <br>

#### Rolling Dice Examples  <br>
A progressive set of examples regarding simulating rolling dice and modeling permutations of doing so. <br>
The article then describes DataTypes and some challenge code.
