# Class 27
## Reading

### [Using Models](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models)
- Django web applications access and manage data through Python objects referred to as models
- Models define the structure of stored data
- Once you've chosen what database you want to use, you don't need to talk to it directly at all 
- you just write your model structure and other code
- Django handles all the dirty work of communicating with the database for you
- When designing your models it makes sense to have separate models for every "object" (a group of related information).
- Models are usually defined in an application's models.py file
- A model can have an arbitrary number of fields, of any type
- each one represents a column of data
- You can declare model-level metadata for your Model by declaring class Meta
- To create a record you can define an instance of the model and then call save()

[Django Admin](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site)
- The Django admin application can use your models to automatically build a site area that you can use to create, view, update, and delete records
- This can save you a lot of time during development, making it very easy to test your models and get a feel for whether you have the right data
- all you must do to add your models to the admin application is to register them
  - Example:
      
        from .models import Author, Genre, Book, BookInstance

         admin.site.register(Book)
         admin.site.register(Author)
         admin.site.register(Genre)
         admin.site.register(BookInstance)
- In order to log into the admin site, we need a user account with Staff status enabled
- You can create a "superuser" account that has full access to the site and all needed permissions using manage.py
- Call the following command, in the same directory as manage.py, to create the superuser:

      python3 manage.py createsuperuser

- To login to the site, open the /admin URL (e.g. http://127.0.0.1:8000/admin) and enter your new superuser userid and password credentials

### [Beginner’s Guide to Django - Part 1](https://simpleisbetterthancomplex.com/series/2017/09/04/a-complete-beginners-guide-to-django-part-1.html)
## Bookmark and Review

### [Beginner’s Guide to Django - Part 2](https://simpleisbetterthancomplex.com/series/2017/09/11/a-complete-beginners-guide-to-django-part-2.html)