# Read 27 - Django Models

#### 2020-08-25

## RESOURCES:
#### Using Models <br>
https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models <br>

#### Django Admin (`Advanced configuration` section is optional) <br>
https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site <br>

#### Beginner’s Guide to Django - Part 1 <br>
https://simpleisbetterthancomplex.com/series/2017/09/04/a-complete-beginners-guide-to-django-part-1.html <br>

#### Beginner’s Guide to Django - Part 2 <br>
https://simpleisbetterthancomplex.com/series/2017/09/11/a-complete-beginners-guide-to-django-part-2.html <br>


## Using Models
__Part 3__ of the __MDN tutorial__ on using Django, and describes how models are defined, and then uses this information to design and implement appropriate models for the LocalLibrary website (*Links to all 11 parts of the tutorial are located on the left sidebar, near the bottom*). <br> 
* A moderate-length read further building out the __*LocalLibrary website*__ tutorial project (begun in earlier installments of this tutorial), __creating separate models for every "object"__ (a group of related information - in this case, books, book instances, and authors) included in the project. <br>
* This article describes __the components of a model__. In a model, __*fields*__ represent __db columns__, and __each field__ can have associated __*arguments*__ and __*types*__ while __models__ can also have __*metadata*__ and __*methods*__. <br>
* __*Every*__ model should have a __`__str__()`__ method as a minimum. <br>
* __Model Management__ describes how to create, modify and search for records.

## Django Admin
__Part 4__ of the __MDN tutorial__ on using Django, focusing on using the __Django Admin site__. A short read (moderate-length read if including the Advanced Configuration material below) further building out the LocalLibrary website tutorial project describiing how to register the models with the admin site, then  how to create and use a login and create some data (e.g., books, genres, book instances, etc.).  <br>
* *__The Django project recommends the Django admin application be used only for internal data management__ (i.e. just for use by admins, or people internal to your organization), as the model-centric approach is not necessarily the best possible interface for all users, and __exposes a lot of unnecessary detail__ about the models.* <br>
* All one __*must*__ do to add one's models to the admin application is to __register__ them. <br>

### (Optional) __Advanced configuration section__ <br>
This section describes adding additional fetures such as __List Views__ and __Detail Views__ to the web UI by using a __`ModelAdmin`__ class (which describes the layout) and register it with the model. <br>
This section further describes how to add various functionality to the project. <br>

---

## (Optional): Beginner’s Guide to Django - Part 1
__Part 1__ of a __7-part series__ on simpleisbetterthancomplex.com <br>
A long read that describes (with visuals and screenshots for clarity) how to get started using Django - from installing prerequisites and Django (in a virtual environment) to getting one's first web page displayed on a local server. <br>

## Beginner’s Guide to Django - Part 2
__Part 2__ of a __7-part series__ on simpleisbetterthancomplex.com <br>
A moderately-long read that extends the project from the first installment (q.v.) and includes plenty of code and visuals. <br>
First, the author walks the reader through some __design considerations__ (i.e., diagramming Use Cases, classes and their relationships and creating Wireframes), then moves into describing Django __Models__, __Views__ and __Templates__, expands to implementing __Static Files__ and __Testing__, and concludes with setting up an __admin account__ to manage it all. <br>
