# Read 09 - Refactoring

#### 2020-03-19

## RESOURCES:
#### Functional Programming Concepts <br>
https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa <br>
#### Refactoring Javascript for Readability <br>
https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hecs <br>

### Functional Programming <br>
The ultimate goal of __Functional Programming__ is to build side-effect-free functions, so it is easier to maintain systems. The first fundamental concept of functional programming is that of "__pure functions__". Here is a very strict definition of purity:
* __*It returns the same result if given the same arguments*__ (it is also referred as 'deterministic') <br>
* __*It does not cause any observable side effects*__ <br>

#### "It returns the same result if given the same arguments" <br>
An __Impure Function__ is one that "__*uses any global object*__ (be it a global variable, an external file, or a random number generated internally) __*that was not passed as a parameter to the function.*__" If the value of the global object changes from one call of the function in question to the next, then the result would be different though the function had the same arguments declared both times. <br>
#### "It does not cause any observable side effects" <br>
"Examples of __observable side effects__ include modifying a global object or a parameter passed by reference."
__*Mutability*__ is discouraged in functional programming (i.e., changing the value of a global object). When data is __immutable__, its state cannot change after it’s created. If you want to change an immutable object, you can’t. *Instead, you create a new object with the new value*.
To make a function pure, simply __have it return the result without modifying the original global object__.
#### Pure functions benefits <br>
The resulting code is easier to test. We don’t need to mock anything.<br>
<br>
### Refactoring Javascript for Readability <br>
This article was a tough read. I caught the gist of what was being expressed, but the examples used were of code problems more advanced than I have used, so the full ramifications of the ideas proposed are lost on me at this point. A good article to revisit later, though.
