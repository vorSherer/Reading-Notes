# Read 06 - Random Numbers and Dependency Injection

#### 2020-05-18

## RESOURCES:
#### How to use Random Module <br>
https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python <br>
#### What is Dependency Injection <br>
https://www.freecodecamp.org/news/a-quick-intro-to-dependency-injection-what-it-is-and-when-to-use-it-7578c84fa88f/ <br>
#### Big O Notation <br>
https://www.youtube.com/watch?v=v4cd1O4zkGw <br>
#### Python Random <br>
https://docs.python.org/3/library/random.html <br>

### How to use Random Module <br>
This is a very quick-and-dirty description for how to use the random module in python, as well a some of its methods such as .randint, .random, .choice, .shuffle and .randrange.

### What is Dependency Injection <br>
"Dependency injection is a technique whereby one object (or static method) supplies the dependencies of another object. A dependency is an object that can be used (a service)." <br>
"Dependencies can be injected at runtime rather than at compile time." <br>
There are basically three types of dependency injection: <br>
1. __Constructor injection__: the dependencies are provided through a class constructor. <br>
2. __Setter injection__: the client exposes a setter method that the injector uses to inject the dependency. <br>
3. __Interface injection__: the dependency provides an injector method that will inject the dependency into any client passed to it. Clients must implement an interface that exposes a setter method that accepts the dependency. <br>
Dependency Inversion There are basically three types of dependency injection:
constructor injection: the dependencies are provided through a class constructor.
setter injection: the client exposes a setter method that the injector uses to inject the dependency.
interface injection: the dependency provides an injector method that will inject the dependency into any client passed to it. Clients must implement an interface that exposes a setter method that accepts the dependency.
Dependency Inversion is the fifth principle of S.O.L.I.D: <br>
__Single-responsibility principle__ - A class should only have a single responsibility, that is, only changes to one part of the software's specification should be able to affect the specification of the class. <br>
__Open–closed principle__ - "Software entities ... should be open for extension, but closed for modification." <br>
__Liskov substitution principle__ - "Objects in a program should be replaceable with instances of their subtypes without altering the correctness of that program." (See also design by contract.) <br> 
__Interface segregation principle__ - "Many client-specific interfaces are better than one general-purpose interface." <br>
__Dependency inversion principle__ - One should "depend upon abstractions, [not] concretions. <br>


### Big O Notation <br>
This was a fairly quick review of Big O with a funny anecdote about a carrier pigeon being faster than an ISP.<br>

### Python Random <br>
Official Python Docs on random. <br>
The numbers generated are only pseudo-random; "Python uses the Mersenne Twister as the core generator. It produces 53-bit precision floats and has a period of 2**19937-1." 
The Mersenne Twister is completely deterministic, it is not suitable for all purposes, and is completely unsuitable for cryptographic purposes. __*The pseudo-random generators of this module should not be used for security purposes!*__
The rest of the documentation categorizes and describes the various functions (methods) of random available. <br>
