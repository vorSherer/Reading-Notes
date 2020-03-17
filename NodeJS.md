# Read 06 - Node, Express, and APIs

#### 2020-03-16

## RESOURCES:
#### An Introduction to Node.js on sitepoint.com <br>
https://www.sitepoint.com/an-introduction-to-node-js/ <br>
#### Node.js Homepage <br>
https://nodejs.org/en/ <br>

   Per the Node.js homepage, *"Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine."*
Stack Overflow expands on this with the cryptic, *"Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library."*

   Per sitepoint; 
*'The creator of Node (Ryan Dahl) took the V8 engine, an open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers, and enhanced it with various features, such as a file system API, an HTTP library, and a number of operating system–related utility methods.*
*This means that Node.js is used to compile JavaScript directly to native machine code that our computer can execute. Hence, it’s a "JavaScript runtime."'*

Node has excellent support for __ECMAScript 2015 (ES6),__ meaning that you don’t generally have to worry about compatibility issues across browsers — as you would if you were writing vanilla JavaScript that would run in different browsers.

Node comes bundled with a package manager called __npm__. This package manager is used to install various JavaScript build tools that can be used for anything from *bundling your JavaScript files and dependencies into static assets*, to *running tests*, or *automatic code linting and style checking*.

Node.js also enables *running JavaScript on the server (Back-end)*. Aside from speed and scalability, an often-touted advantage of using JavaScript on a web server — as well as in the browser — is the added benefit that you can do everything in the same language.
Node also speaks __JSON__, one of the most common data exchange formats on the web, *without the need for reformatting*. You can have one syntax from browser to server to database.

In very simplistic terms, when you connect to a traditional server, such as __Apache__, it will spawn a new thread to handle the request. In a language such as __PHP__ or __Ruby__, any subsequent I/O operations (for example, interacting with a database) *block the execution of your code until the operation has completed*. 
Node.js, however, is __single-threaded__. It’s also __event-driven,__ which means that everything that happens in Node is in reaction to an event. For example, when a new request comes in (one kind of event) the server will start processing it. If it then encounters a blocking I/O operation, *instead of waiting for this to complete,* it will register a __callback__ before continuing to process the next event. When the I/O operation has finished (another kind of event), the server will execute the callback and continue working on the original request. Under the hood, Node uses the __libuv__ library to implement this asynchronous (that is, non-blocking) behavior.

Sitepoint's conclusion; "There are many other exciting and varied uses of Node.js! For example it can be used as a scripting language to automate repetitive or error prone tasks on your PC. It can also be used to write your own command line tool, such as this Yeoman-Style generator (see Sitepoint artical, above, for the link) to scaffold out new projects. Node.js can also can be used to build cross-platform desktop apps and even to create your own robots."

