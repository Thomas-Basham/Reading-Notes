# Class 32
## Readings: Authentication & Production Server

### [JSON Web Tokens](https://jwt.io/introduction/)
- JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object
- This information can be verified and trusted because it is digitally signed
- JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
- In its compact form, JSON Web Tokens consist of three parts separated by dots (.), which are:
    
        Header
        Payload
        Signature
- The output is three Base64-URL strings separated by dots that can be easily passed in HTML and HTTP environments, while being more compact when compared to XML-based standards such as SAML
- Whenever the user wants to access a protected route or resource, the user agent should send the JWT, typically in the Authorization header using the Bearer schema. The content of the header should look like the following:

        Authorization: Bearer <token>

### [DRF JWT Authentication](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)
- The JWT is just an authorization token that should be included in all requests:

        curl http://127.0.0.1:8000/hello/ -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1Ni
- The JWT is acquired by exchanging an username + password for an access token and an refresh token
- The access token is usually short-lived (expires in 5 min or so, can be customized though)
- The refresh token lives a little bit longer (expires in 24 hours, also customizable). It is comparable to an authentication session
- After it expires, you need a full login with username + password again
- pip install djangorestframework_simplejwt
- settings.py:

        
        REST_FRAMEWORK = {
            'DEFAULT_AUTHENTICATION_CLASSES': [
                'rest_framework_simplejwt.authentication.JWTAuthentication',
            ],
        }
- urls.py:

        
        from django.urls import path
        from rest_framework_simplejwt import views as jwt_views
        
        urlpatterns = [
            # Your URLs...
            path('api/token/', jwt_views.TokenObtainPairView.as_view(), name='token_obtain_pair'),
            path('api/token/refresh/', jwt_views.TokenRefreshView.as_view(), name='token_refresh'),
        ]


### [Django Runserver Is Not Your Production Server](https://build.vsupalov.com/django-runserver-in-production/)
- You want to only use tech in production, which is reliable, well tested and has been around for a while
- When a request arrives at your server, it should be passed to a dedicated web server. Nginx is an example for a good web server
- Your Django app does not actually run as you would think a server would - waiting for requests and reacting to them
- Your project provides a uwsgi.py file, which contains a function to be called by the application server
- If you want to run Django in production, be sure to use a production-ready web server like Nginx
- and let your app be handled by a WSGI application server like Gunicorn.
## Videos

### [JWT with DRF](https://www.youtube.com/watch?v=Fhcn2qx-4VQ)
## Bookmark and Review

### [Gunicorn](https://gunicorn.org/)

### [Django Migrations Primer](https://realpython.com/django-migrations-a-primer/)
