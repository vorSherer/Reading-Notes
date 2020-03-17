# Read 07 - APIs continued

#### 2020-03-17

## RESOURCES:
#### What Google Learned From Its Quest to Build the Perfect Team <br>
https://www.nytimes.com/2016/02/28/magazine/what-google-learned-from-its-quest-to-build-the-perfect-team.html <br>
#### How I explained REST to my brother <br>
https://gist.github.com/brookr/5977550 <br>
#### Documentation for SuperAgent <br>
https://visionmedia.github.io/superagent/ <br>

### Teams
In the article "*What Google Learned From Its Quest to Build the Perfect Team*," some high points were: 
"studies show that __groups tend to innovate faster, see mistakes more quickly and find better solutions to problems (than individuals)__... (and) that __people working in teams tend to achieve better results and report higher job satisfaction.__"
"No matter how researchers arranged the data, though, it was almost impossible to find patterns — or any evidence that the composition of a team made any difference.... __The ‘who’ part of the equation didn’t seem to matter.__"
(Google's Project Aristotle) "researchers eventually concluded that what distinguished the ‘good’ teams from the dysfunctional groups was __how teammates treated one another.__"
"...on the good teams, members spoke in roughly the same proportion... ‘As long as everyone got a chance to talk, the team did well,’ Woolley said. ‘But if only one person or a small group spoke all the time, the collective intelligence declined.’"
"...__the good teams all ... were skilled at intuiting how others felt__ based on their tone of voice, their expressions and other nonverbal cues."
"For Project Aristotle, research on __psychological safety__ pointed to particular norms that are vital to success. There were other behaviors that seemed important as well — like making sure teams had clear goals and creating a culture of dependability. But Google’s data indicated that __psychological safety, more than anything else, was critical to making a team work." "In the best teams, members listen to one another and show sensitivity to feelings and needs."__

*****************************************
### REST
__REST__ stands for __*Representational State Transfer*__. (It is sometimes spelled "ReST".)
"The whole world wide web is built on an architectural style called '__REST__'."
__*Rest is a protocol to exchange any(XML or JSON) messages that can use HTTP to transport those messages.*__
A web page is a “representation” of a resource, so are “__Web Services__” or "__APIs__". 
Computers can use (HTTP) to send messages back and forth to each other. We need some way of having one machine tell another machine about a resource that might be on yet another machine. This is done using a '__redirect__.'
When you go to a web page, the browser does an __HTTP GET__ on the URL you type in and back comes a web page. Web pages usually have images and those are separate resources. *"The web page just specifies the URLs to the images and the browser goes and does more GETs using the HTTP protocol on them until all the resources are obtained and the web page is displayed. But the important thing here is that very different kinds of nouns can be treated the same. Whether the noun is an image, text, video, an mp3, a slideshow, whatever. I can GET all of those things the same way given a URL."*
"When a machine GETs the resource, it will ask for the machine readable one. When a browser GETs a resource for a human, it will ask for the human readable one."

*****************************************
### Superagent
Superagent is a node library that will simplify our URL requests. Each URL request will be "wrapped in a superagent call" to handle the heavy lifting of obtaining the desired resources.
