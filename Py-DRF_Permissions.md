# Read 32 - Django REST Framework (DRF) and PostgreSQL

#### 2020-09-12

## RESOURCES:
### DRF Permissions <br>
https://www.django-rest-framework.org/api-guide/permissions/ <br>
#### Sublinks:
- __*Authentication*__ - https://www.django-rest-framework.org/api-guide/authentication/ <br>
- __*Throttling*__ - https://www.django-rest-framework.org/api-guide/throttling/ <br>
- __*Filtering*__ - https://www.django-rest-framework.org/api-guide/filtering/ <br>


### Classy Django REST <br>
http://www.cdrf.co/ <br>
#### Related Link:
- Classy Class-Based Views <br>
http://www.ccbv.co/ <br>


### DRF Generic Views <br>
https://www.django-rest-framework.org/api-guide/generic-views/ <br>


---

## DRF Permissions <br>
This medium-length read describes how permissions work, how to assign them in various instances, and concludes with a listing of third-party packages that can be applied in specialized instances. <br>
> *Authentication or identification by itself is not usually sufficient to gain access to information or code. For that, the entity requesting access must have authorization.* <br>
	-- *Apple Developer Network* <br>

__Authentication__, __Permissions__ and __Throttling__ together determine whether a request should be granted or denied access. <br>
- __*Authentication*__ associates an incoming request with a set of identifying credentials. <br>
- __*Permissions checks*__ then determine if the incoming request should be permitted. Permissions are used to grant or deny access for different classes of users to different parts of the API. Permissions may be set at the __view-level__ or at the __object-level__ or lower. <br>
- __*Throttling*__ also determines if a request should be authorized. __Throttles__ indicate a temporary state, and are used to control the rate of requests that clients can make to an API. <br>


---

## Classy Django REST <br>
This is an excellent ToC-type reference list of outlinks to visual summaries of DRF Tools, with any available methods and attributes to each listed and described. <br>

---

## DRF Generic Views <br>
A long-ish read describing what is made available through the __`rest_framework/generics`__ toolset. <br>
__"Generics"__, as the name implies, simplifies development by providing a number of pre-built views that provide for commonly used patterns. Various components can be combined to further define a tailored view without having to resort to a purely custom-built solution. <br>
