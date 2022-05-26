# Class 31

## Reading

### [Beginner’s Guide to Docker](https://wsvincent.com/beginners-guide-to-docker/)

- Docker is a way to isolate and run entire applications
- The entire development environment is isolated: programming language, software packages, databases, and more
- Docker is really just Linux containers which are a type of virtualization
- Inspect Docker with 
      
      $ docker info

- Inspect Docker Image 

      $ docker image ls

- We can create an image and container just for Python and later add on to it
- Add this in Dockerfile:
     
      $ FROM python:3.7-alpine

- Build Image
      
      $ docker image build .

- docker-compose.yml is a list of container instructions

      $ pipenv install django==3.0
      $ pipenv shell
      $ django-admin startproject example_project .
      $ touch Dockerfile
      $ touch docker-compose.yml
- Inside docker file:

      # Dockerfile

      # Python version
      FROM python:3.7-alpine
    
      # Set environment variables
      ENV PYTHONDONTWRITEBYTECODE 1
      ENV PYTHONUNBUFFERED 1
    
      # Set work directory
      WORKDIR /code
    
      # Install dependencies
      COPY Pipfile Pipfile.lock /code/
      RUN pip install pipenv && pipenv install --system
    
      # Copy project
      COPY . /code/
- Order matters in Dockerfiles since they are executed from top-to-bottom
- In the yml:
 
      # docker-compose.yml
      version: '3.7'
    
      services:
        web:
          build: .
          command: python /code/manage.py runserver 0.0.0.0:8000
          volumes:
            - .:/code
          ports:
            - 8000:8000
- THEN:
 
       $ docker-compose up --build

### [Django for APIs - Library Website](https://djangoforapis.com/library-website-and-api/)

- Django REST Framework works alongside the Django web framework to create web APIs 

      $ python -m pip install djangorestframework~=3.13.0

      INSTALLED_APPS = [
          "django.contrib.admin",
          "django.contrib.auth",
          "django.contrib.contenttypes",
          "django.contrib.sessions",
          "django.contrib.messages",
          "django.contrib.staticfiles",
          # 3rd party
          "rest_framework",  # new
          # Local
          "books.apps.BooksConfig",
          "apis.apps.ApisConfig",  # new
      ]
## Bookmark and Review

### [Beginner’s Guide to Django REST Framework](https://wsvincent.com/official-django-rest-framework-tutorial-beginners-guide)