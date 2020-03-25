# Read 13 - "Update/Delete" (but actually GET/POST)

#### 2020-03-25

## RESOURCES:
#### Sending Form Data (MDN) <br>
https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data <br>
#### HTML5 Forms Reference <br>
https://htmlreference.io/forms/ <br>
#### Video Series on Styling HTML5 Forms <br>
https://www.youtube.com/playlist?list=PL4cUxeGkcC9g5_p_BVUGWykHfqx6bb7qK <br>

Despite the Reading title today of "Update/Delete," the reading actually covered HTTP __GET__ and __POST__ methods, which set the background for understanding Updates (using __PUT__ or __PATCH__ ) and __DELETE__. <br>
### Sending Form Data
The first article, "__*Sending Form Data*__" opens with a summary of client/server communication used by the internet, summarized as follows. <br>
A __*client*__ (usually a web browser) sends a __*request*__ to a server, using the __*HTTP protocol*__. The __*server*__ answers the request (__*responds*__) using the same protocol. <br>
### The Client Side <br>
An __*HTML form*__ on a web page transforms a __*user request*__ into an HTTP request to send that data to a server when the user hits a __*submit button*__. <br>
<br>
The ```<form>``` element includes __*attributes*__ that configure the request.  The two most important attributes are ```action``` and ```method```. <br>
<br>
The ```action``` attribute defines _where the data gets sent_. Its __value__ must be a __valid relative or absolute URL__.
The __names__ and __values__ of the *form controls* are sent to the server as ```name=value``` pairs joined with ampersands in the HTTP request. The ```action``` value should be *a file on the server* that can handle the incoming data, including ensuring server-side validation. <br>
<br>
The server then responds, generally handling the data and loading the URL defined by the ```action``` attribute, causing a new page load (or a refresh of the existing page, if the action points to the same page). <br>
<br>
The ```method``` attribute defines *how data is sent*, the most common being the ```GET``` method and the ```POST``` method. <br>
<br>

The ```GET``` method is used by the browser to send the form information to the server *as URL parameters*: The data is appended to the URL after a question mark (```?```), followed by the __name/value pairs__ ("name=value"), each pair separated by an __ampersand__ (```&```). __The key point to note here is that *the data is visible in the HTTP string*.__
<br>

The ```POST``` method differs in that the form information is sent to the server *as part of the request body*. If a form is sent using this method, the data is __appended within the body of the HTTP request__ (a more secure form of transmission). <br>

### Meanwhile, back at the server... <br>
Whichever HTTP method one chooses, *the server receives a string that will be __parsed__* in order to get the data as a list of *name/value pairs*. The way one accesses this list depends on the __*development platform*__ one uses and on any specific __*frameworks*__ one may be using with it. <br>
<br>

There are many server-side technologies one can use for form handling, including __Perl, Java, .Net, Ruby__, etc. One may select any that one prefers, but it is not likely to be used alone. It's more common to use a corresponding high quality __framework__ to make handling forms much easier than trying to write all the functionality oneself from scratch, and will save a lot of time. Some commonly-used frameworks include: <br>
* __Django__ for __Python__. <br>
* __Express__ for __Node.js__. <br>
* __Laravel__ for __PHP__. <br>
* __Ruby On Rails__ for __Ruby__. <br>
<br>

### Security issues. <br>
Each time one sends data to a server, one needs to consider security. HTML forms are by far the most common server __attack vectors__. <br>
To fight these threats, *the most important rule is:* __never ever trust your users, including yourself__; even a trusted user could have been hijacked. *All data* that comes to your server *must be __checked__ and __sanitized__*. *Always. No exceptions.*  <br>
#### How? (Verbatim recommendations below.)
* __Escape potentially dangerous characters.__ The specific characters you should be cautious with vary depending on the context in which the data is used and the server platform you employ, but all server-side languages have functions for this. <br>
* __Limit the incoming amount of data__ to allow only what's necessary. <br>
* __Sandbox uploaded files__. Store them on a different server and allow access to the file only through a different sub-domain or even better through a completely different domain. <br>
* __Have a periodic security review__ performed by a competent third party. <br>

### In Summary
Sending form data is easy, but securing an application can be tricky. Just remember that a front-end developer __*is not*__ the one who should define the security model of the data. It's possible to perform *client-side form validation*, but *the server can't trust that this validation has been done, or done correctly!*
