# Read 03 - Files in Python

#### 2020-05-13

## RESOURCES:
#### Read & Write Files in Python
https://realpython.com/read-write-files-python/ <br>
#### Exceptions in Python
https://realpython.com/python-exceptions/ <br>
#### Video: Read & Write Files in Python - Companion Video
https://realpython.com/courses/reading-and-writing-files-python/ <br>
#### Reading and Writing Files in Python Quiz <br>
https://realpython.com/quizzes/read-write-files-python/ <br>

#### Read & Write Files in Python
Files on most modern file systems are composed of three main parts: <br>
* Header: metadata about the contents of the file (file name, size, type, and so on) <br>
* Data: contents of the file as written by the creator or editor <br>
* End of file (EOF): special character that indicates the end of the file <br>
Windows uses the CR+LF characters to indicate a new line, while Unix and the newer Mac versions use just the LF character. This can cause some complications when you’re processing files on an operating system that is different than the file’s source. <br>
When you want to work with a file, the first thing to do is to open it by invoking the open() built-in function. <br>
After you open a file, the next thing to learn is how to close it: <br>
* The first way to close a file is to use the try-finally block (q.v.) <br>
* The second (better) way to close a file is to use the with statement: "with open('filename.txt') as reader: " The with statement automatically takes care of closing the file once it leaves the with block, even in cases of error. <br>
**  you’ll also want to use the second positional argument, mode (q.v.) - the most common of which is "r": <br>
**     with open('dog_breeds.txt', 'r') as reader: <br>
**         # Further file processing goes here. <br>
Opened files may be read using ".read(size=-1)", ".readline(size=-1)", or "readlines()".

#### Exceptions in Python
A Python program terminates as soon as it encounters an error. In Python, an error can be a syntax error or an exception. Syntax errors occur when the parser detects an incorrect statement. An exception error occurs whenever syntactically correct Python code results in an error. <br>
The try and except block in Python is used to catch and handle exceptions. <br>
