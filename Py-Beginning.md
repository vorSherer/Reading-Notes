# Read 01 - Beginning Python 401

#### 2020-05-10

## RESOURCES:
#### Pain and Suffering <br>
https://codefellows.github.io/code-401-python-guide/curriculum/class-01/notes/pain_suffering <br>
#### Beginners Guide to Big O <br>
https://rob-bell.net/2009/06/a-beginners-guide-to-big-o-notation/ <br>
#### Season 1, Episode 6, A friendly intro to Big O Notation <br>
https://www.codenewbie.org/basecs/8 <br>
#### Names and Values in Python <br>
https://www.youtube.com/watch?v=_AEJHKGk9ns <br>
#### Awesome Python Environment <br>
https://towardsdatascience.com/how-to-setup-an-awesome-python-environment-for-data-science-or-anything-else-35d358cc95d5 <br>
#### Python Module of the Week <br>
https://pymotw.com/3/index.html <br>
<br>

### Pain and Suffering
Better entitled "Pain versus Suffering" - Pain is common, mostly unavoidable, and best met with a clear head and a mind to press through. Suffering describes all other pain - pain without purpose, avoidable pain, unnecessarily-extended pain, etc. <br>
<br>
#### Key Take-aways on Pain versus Suffering:
Pain is coming in this course: Plan for it, set your mind to learn to work through it, remember the ultimate goal (i.e., why you're doing this). Don't let it devolve to suffering. <br>
<br>

### A beginner's guide to Big O notation
Big O notation is used in Computer Science to describe the performance or complexity of an algorithm. Or, put more simply, comparing certain features of a coding solution to determine how much space (in memory) and how much (processing) time the code will take to perform certain functions, how often it will be called upon to perform those functions, and how the cumulative amount of those time and space factors grow when taken to very large scale applications. There is no "one-size-fits-all" solution to Big O; the mix for one code solution for a given application likely won't fit a different solution for a different application. Big O must be evaluated on a case-by-case basis. <br>
<br>
#### Key Take-aways on Big O Notation:
Big O notation is a customized logarithmic evaluation of several performance characteristics of a given code algorithm to determine the processing time and memory space trade-offs as the solution is applied to very large-scale applications. <br>
<br>

### A friendly intro to Big O Notation
A very simplified explanation of what Big O notation measures, and uses a singly linked list data structure to illustrate the differences. <br>
<br>
#### Key Take-aways on Big O Notation:
Big O notation is applied to several functions of an algorithm to determine how these various operations perform and how that changes as the scale is increased, taking into consideration how often each operation will need to be performed. <br>
<br>

### Names and Values in Python
Details about names, values, assignment and mutability; <br>
Names refer to values, many names can refer to the same value, but reassigning one of those names doensn't change the value of the other(s).
Values live until they are no longer referred to.
Assignment never copies data; it only creates another reference to an existing value.
Mutating a list makes the changes visible to all names that refer to the same list.
Immutable values cannot alias.
"Changing" an int is actually re-binding the name to a new value.
"Changing" a list is actually mutating the list.
In Python, Names have scope, but no type, while values have type, but no scope.
Python is "call-by-assignment" rather than call-by-value or call-by-reference.  <br>
<br>
#### Key Take-aways on Names and Values in Python:
Understand what is going on under the hood (with python, or any language) to avoid surprises that arise from assumptions of how things work. <br>
<br>

### How to Setup an Awesome Python Environment
Pyenv allows one to support one program with different python versions or different versions of the same third-party library and to switch between them seemlessly.
Poetry is one tool used to manage project dependencies.
Black is a tool that automates code formatting.
Mypy is a static type=checking tool for python code.
Pre-commit is a tool that executes checks before permitting one to make a git commit. When those checks fail, your commit will be rejected. <br>
<br>
#### Key Take-aways on Python Environment tools:
There are many tools around that help you focus on what is important - content. Find the tools that work for you and learn how to configure and use them properly so they take care of the "side-jobs" and let you focus on the code. <br>
<br>

### Python 3 Module of the Week
PyMOTW-3 is a series of articles written by Doug Hellmann to demonstrate how to use the modules of the Python 3 standard library. It is based on the original PyMOTW series, which covered Python 2.7. <br>
<br>
#### Key Take-aways on TOPIC:
This is a fabulous reference to be kept handy as one develops one's skill with Python.
