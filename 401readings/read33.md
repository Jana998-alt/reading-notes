# Authentication & Production Server 

## JSON Web Tokens 

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.

it is used for authorization and information extchange.

In its compact form, JSON Web Tokens consist of three parts separated by dots (.), which are:

- Header
- Payload
- Signature

```xxxxx.yyyyy.zzzzz```

which is called:  a **token**.

Whenever the user wants to access a protected route or resource, the user agent should send the JWT, typically in the Authorization header using the Bearer schema. The content of the header should look like:

```Authorization: Bearer <token>```

## Using JWT with django-rest-framework

2 types of tokens:

The access token is usually short-lived.
The refresh token lives a little bit longer. It is comparable to an authentication session. After it expires, you need a full login with username + password again.

in settings.py, add: 
```
REST_FRAMEWORK = {
    'DEFAULT_AUTHENTICATION_CLASSES': [
        'rest_framework_simplejwt.authentication.JWTAuthentication',
    ],
}
```

in urls, add:

```
urls.py

from django.urls import path
from rest_framework_simplejwt import views as jwt_views

urlpatterns = [
    # Your URLs...
    path('api/token/', jwt_views.TokenObtainPairView.as_view(), name='token_obtain_pair'),
    path('api/token/refresh/', jwt_views.TokenRefreshView.as_view(), name='token_refresh'),
]
```
the url that you pass to access the protected infromation should look like:

http http://127.0.0.1:8000/hello/ "Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNTQ1MjI0MjAwLCJqdGkiOiJlMGQxZDY2MjE5ODc0ZTY3OWY0NjM0ZWU2NTQ2YTIwMCIsInVzZXJfaWQiOjF9.9eHat3CvRQYnb5EdcgYFzUyMobXzxlAVh_IAgqyvzCE"

## Django Runserver Is Not Your Production Server

the server started with runserver is not guaranteed to be performant (it’s very slow), and it hasn’t been built with security concerns in mind. Not a good fit for production use.

the right way to test that is through: production stack

it is the organisation stage between securing a project and delivering it. It focuses on helping your business stay on top of project budgets, resources and timelines.
