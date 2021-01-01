# django-rest-custom-authentication-example


This is example of custom JWT token authentication. 

This will be check every request. The request have a token with in HTTP header.

The authentication.py file override override the .authenticate(self, request) method.

You should add authentication.py to the foler with setting.py

and add below code in setting.py 

!Note! : you should change yourappname 



REST_FRAMEWORK = 

{
    
    "DEFAULT_AUTHENTICATION_CLASSES": [
    
    "yourappname.authentication.JWTBaseAuthentication",
        
    ],
}


 
