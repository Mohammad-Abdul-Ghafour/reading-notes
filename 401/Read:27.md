# Authentication & Production Server

## JWT :
* JWT is shortcut for JSON Web Tokens
*  an open standard used to share security information between two parties — a client and a server. 
* Each JWT contains encoded JSON objects, including a set of claims. 
* JWTs are signed using a cryptographic algorithm to ensure that the claims cannot be altered after the token is issued.
* JWT consists of:

![](https://uploads.toptal.io/blog/image/956/toptal-blog-image-1426676395222.jpeg)

## JWT vs Cookies:

![](https://nileshprasad137.github.io/assets/blogimg/tokenadv.jpg)

## Why use JWT:
* it is fast for transmission and usable.
* Self Content
* It contains the details of user
* Tokens can be generated from anywhere.


## JWT Authentication and Django REST Framework

![](https://miro.medium.com/max/960/1*l-FS80RhxUgjZOKGgOXnTQ.jpeg)

## Using JWT with Rest framework:
```
from django.urls import path, include
from rest_framework_simplejwt import views as jwt_views

urlpatterns = [
	path('api/token/',
		jwt_views.TokenObtainPairView.as_view(),
		name ='token_obtain_pair'),
	path('api/token/refresh/',
		jwt_views.TokenRefreshView.as_view(),
		name ='token_refresh'),
	path('', include('app.urls')),
]

```


### References:
[JWT documentation](https://jwt.io/introduction/)
[using jwt with REST framework](https://www.geeksforgeeks.org/jwt-authentication-with-django-rest-framework/)