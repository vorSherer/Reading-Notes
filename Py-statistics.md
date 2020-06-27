# Read 09 - Dunders, Statistics and non-attribution

#### 2020-06-27

## RESOURCES:
#### Dunder Methods <br>
https://dbader.org/blog/python-dunder-methods <br>
#### Statistics - Probability <br>
https://www.dataquest.io/blog/basic-statistics-in-python-probability/ <br>
#### Video: Intro to Statistics <br>
https://www.youtube.com/watch?v=MdHtK7CWpCQ <br>
#### Video: AI Guru makes $238,800 with misleading paid course, doesn’t credit developers <br>
https://www.youtube.com/watch?v=7jmBE4yPrOs <br>
#### Statistics Module <br>
https://docs.python.org/3/library/statistics.html <br>



### Dunder Methods <br>
In Python, special methods are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores, for example __\_\_init\_\___ or __\_\_str\_\___. Pythonistas adopted the term __*“dunder methods”*__, a short form of *“double under.”* Dunder methods let you emulate the behavior of built-in types, e.g., <br>
Object Initialization: __*'__init\__'*__ - The *\_\_init\_\_* constructor takes care of setting up the object.  <br>
Object Representation: __'\_\_str\_\_', '\_\_repr\_\_'__; <br>
* __*\_\_repr\_\_*__: The “official” string representation of an object. This is how you would make an object of the class. The goal of \__repr\__ is to be unambiguous. <br>
* __*\_\_str\_\_*__: The “informal” or nicely printable string representation of an object. This is for the enduser. <br>
If you wanted to implement just one of these to-string methods on a Python class, make sure it’s __*\_\_repr\_\_*__. <br>
Iteration: __'\_\_len\_\_', '\_\_getitem\_\_', '\_\_reversed\_\_'__ - In it's native form, a class in python is not iterable. Using these dunder methods can change that. e.g., <br>

def \_\_len\_\_(self): <br>
.  return len(self._transactions)

def __getitem__(self, position): <br>
.  return self._transactions[position]
'''
<br>

### Statistics - Probability <br>
This reading served up the fundamentals of statistics, covering __probability__ (the chance of an event happening), the role of __statistics__ in determining probability, described __distribution curves__ for each, and the roles of the __*Central Limit Theorem*__ and __*the Three Sigma Rule*__ in *normalizing* distribution. <br>


### Video: Intro to Statistics <br>
This YouTube video was an introduction to the fundamentals of statistics, presented by an over-animated presenter.  Not sure how much this video was chosen for its content, or how much it was selected as grist for the next video (q.v.). <br>


### Video: AI Guru makes $238,800 with misleading paid course, doesn’t credit developers <br>
Presented as an extreme example of "non-attribution of code," this YouTube video was a long exposé on the presenter of the first video, exposing the extent of his ripping off the code originated by another, claiming it as his own original work, and then later claiming the original work as "starter code" to which he is reputed to only have added an original README. <br>


### Statistics Module <br>
This is python documentation on ways to use statistical methods in one's code. <br>
