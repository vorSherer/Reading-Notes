# Read 29 - Django Custom User

#### 2020-09-01

## RESOURCES:
### Django Custom User Model <br>
https://learndjango.com/tutorials/django-custom-user-model <br>
### Creating a Custom User Model <br>
https://www.youtube.com/watch?v=eCeRC7E8Z7Y&t=59s <br>
### Abstract User, User Profile and Signals in Django <br>
https://www.youtube.com/watch?v=EudKs1HPUfE <br>
### Substituting a custom User model <br>
https://docs.djangoproject.com/en/3.0/topics/auth/customizing/#auth-custom-user <br>

---

## Django Custom User Model <br>
"Django ships with a built-in User model for authentication, however the official Django documentation *highly recommends* using a custom user model for new projects" because "updating the default User model in an existing Django project is very, very challenging."  <br>
Describes step-by-step how to creaate a custom user in a non-poetry way. <br>
#### Additional Link:
[How to implement a regular login, logout, signup flow in Django](https://learndjango.com/tutorials/django-login-and-logout-tutorial)

---

## Creating a Custom User Model <br>
A __CodingWithMitch__ YouTube video (22 min. long) that describes an alternate method to build a custom user model using __`AbstractBaseUser`__ and __`BaseUserManager`__. <br>
