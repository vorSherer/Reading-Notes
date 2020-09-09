# Read 31 - Django REST Framework and Docker

#### 2020-09-08

## RESOURCES:
#### Beginner’s Guide to Docker <br>
https://wsvincent.com/beginners-guide-to-docker/ <br>

#### Django for APIs - Library Website
	(May ask you for email because it’s a sample chapter for (fantastic) book they’re selling)
https://djangoforapis.com/library-website-and-api/ <br>

#### Beginner’s Guide to Django REST Framework <br>
https://learndjango.com/tutorials/official-django-rest-framework-tutorial-beginners <br>

---
---

## Beginner’s Guide to Docker <br>
A long-ish read by Wm. Vincent on Docker. <br>
Docker is really just Linux containers which are a type of virtualization, as are virtual environments (venv), which can only isolate Python software packages locally. <br>
Conversely, with Docker one can run a production database or other services within self-contained, platform -independent Docker containers. <br>
__Images__ and __containers__ are the two fundamental concepts to grasp when you start with Docker. __An image__ is a snapshot in time of what a project contains. __A container__ is a running instance of the image. <br>

*"A baking analogy we can use here is as follows:
	- A __Dockerfile__ is the recipe for a cake
	- An __image__ is a snapshot of the recipe at a given time 
	- A __docker-compose.yml__ says how to make the cake
	- And the __container__ is the actual, baked cake"* <br>
Docker caches the steps in a Dockerfile to speed up subsequent builds. __*When a change is made to a step, all steps following it will be executed from scratch*__. For this reason, order matters in a Dockerfile. Typically you want to put code that won’t change often at the top and code that will change at the end. <br>

---

## Django for APIs - Library Website 
A long-ish read on implementing Django REST Framework for creating web API's. <br>
*"The most important takeaway is that __Django creates websites__ containing webpages, while __Django REST Framework creates web APIs__ which are a collection of URL endpoints containing available HTTP verbs that return JSON.* <br>
This tutorial uses Django to build out a basic Library web site, then extends it into a web API with Django REST Framework. <br>

---

## Beginner’s Guide to Django REST Framework <br>
A long-read, newbie-friendly version of the official Django Rest Framework tutorial by Wm. Vincent. 
A few of the steps still assume beyond-newbie familiarity with the particulars, but the tutorial is, overall, easy to understand and execute. <br>

---
