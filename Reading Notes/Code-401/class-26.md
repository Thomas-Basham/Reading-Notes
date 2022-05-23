# Class 26
## Reading

### [Getting started with Django](https://www.djangoproject.com/start/)
- Django provides an abstraction layer (the “models”) for structuring and manipulating the data of your web application
- Example:
    
      from django.db import models
 
      class Person(models.Model):
          first_name = models.CharField(max_length=30)
          last_name = models.CharField(max_length=30)
  
- Django has the concept of “views” to encapsulate the logic responsible for processing a user’s request and for returning the response

- Example: Here’s a sample URLconf:
        
        from django.urls import path
        
        from . import views
        
        urlpatterns = [
            path('articles/2003/', views.special_case_2003),
            path('articles/<int:year>/', views.year_archive),
            path('articles/<int:year>/<int:month>/', views.month_archive),
            path('articles/<int:year>/<int:month>/<slug:slug>/', views.article_detail),
        ]

- The template layer provides a designer-friendly syntax for rendering the information to be presented to the user
- Templates in Django are similar to Jinja Templates in Flask
- Django provides a rich framework to facilitate the creation of forms and the manipulation of form data
- One of the most powerful parts of Django is the automatic admin interface
- It reads metadata from your models to provide a quick, model-centric interface where trusted users can manage content on your site
- Security is a topic of paramount importance in the development of web applications and Django provides multiple protection tools and mechanisms

### [How Django Works Behind the Scenes](https://wsvincent.com/how-django-works-behind-the-scenes/)

- Django was originally developed at the Lawrence Journal-World newspaper by Adrian Holovaty, Simon Willison, and Jacob Kaplan-Moss
- The code was open-sourced in 2005 and developers immediately started making contributions to the codebase
- Django is maintained by a non-profit company called the Django Software Foundation
- The Django Fellows Program are paid contractors who triage tickets, manage releases, and other Django maintenance 

## Bookmark and Review

### [What is Django](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Introduction)
- Django is a high-level Python web framework that enables rapid development of secure and maintainable websites
- Django helps you write software that is:
  - Complete
  - Versatile
  - Secure
  - Scalable
  - Maintainable
  - Portable
  
### [First Django App - Part 1](https://docs.djangoproject.com/en/3.0/intro/tutorial01/)

### [First Django App - Part 2](https://docs.djangoproject.com/en/3.0/intro/tutorial02/)