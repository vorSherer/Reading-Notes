# Read 10 - The Call Stack and Debugging

#### 2020-03-20

## RESOURCES:
#### The Call Stack defined on MDN <br>
https://developer.mozilla.org/en-US/docs/Glossary/Call_stack <br>
#### Understanding the JavaScript Call Stack <br>
https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/ <br>
#### JavaScript error messages <br>
https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c <br>
#### JavaScript errors reference on MDN <br>
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors <br>


### The Call Stack
"A call stack is a *data structure* that uses the __Last In, First Out (LIFO)__ principle to temporarily store and manage *function invocation (call)*." It is "a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions..."
"When a script calls a function, the __interpreter__ adds it to the __call stack__ and then starts carrying out the function."
"When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a __stack frame__. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it is popped out of the stack."
"Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
If the stack takes up more space than it had assigned to it, it results in a "__stack overflow__" error." This can also happen "when there is a recursive function (a function that calls itself) without an exit point."
#### EXAMPLE:
So if a script is being run and a function is called (*function 'A'*), the interpreter adds it to the call stack. Well, that function calls (invokes) another function as part of its purpose (*function 'B'*), so the interpreter adds that to the call stack above function 'A'. The interpreter will try to execute function 'B' first, because function 'A' is "on hold" until function 'B' completes. If function 'B' calls *function 'C'* which calls *function 'D'*, then the interpreter runs them in reverse order (D, C, B, A), clearing each one off the call stack as soon as it completes, then resuming where it left off with the next function down and so on until all are completed and removed from the call stack.
"We started with an empty Call Stack, and whenever we invoke a function, it is automatically added to the Call Stack, after executing all of its codes, it is automatically removed from the Call Stack. At the end, we ended up with an empty stack too."

#### Key Take-aways on the Call Stack:
1. It is __*single-threaded*__. Meaning it can only do one thing at a time.
2. Code execution is __*synchronous*__.
3. A function invocation creates a __*stack frame*__ that occupies a temporary memory.
4. It works as a __*LIFO*__ — Last In, First Out data structure.
5. As a stack frame completes, it is popped off of the Call Stack.

### Debugging
In the very early days of electronics, odd failures could be caused by insects ("bugs") getting inside and either eating through insulation or getting themselves electrocuted as they short-circuited one or more components. Repair techs began to refer to "bugs" in the machine as a catch phrase for any circuit failure.  That terminology was adopted by programmers as computers came along to refer to any errors in the code. 
#### Types of programming errors: <br>
__Reference errors__ - This is as simple as when you try to use a variable that is not yet declared. <br>
__Syntax errors__ - this occurs when you have something that cannot be parsed in terms of syntax (i.e., the code is incomplete or incorrectly written). <br>
__Range errors__ - A numeric value is outside of the allowable range. This can happen if trying to manipulate an object with some kind of length and giving it an invalid length. <br>
__Type errors__ - This type of errors occurs when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable. <br>

If an error occurs and in left __unhandled__, all code execution stops. (*Windows BSOD, anyone?*) This can be avoided by __*providing some form of error handling*__ in the code ("if something goes wrong, do this"), so that the interpreter has a way of setting the error aside and continuing it's tasks with the rest of the code. Implementing a "__Try...Catch__" structure is an example of an effective option for accomplishing this.

With __*Complied Languages*__ (like Java), errors can occur during __complilation__ or at __runtime__. __*Non-compiled Languages*__ (like JavaScript) only reveal their errors at runtime.
