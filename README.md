# django-howto
Django Howtos tutorial

Notes Covered: MySite
Part 1
Creating a django project
 django-admin startproject mysite

Run the server
 python manage.py runserver

Creating an app
 python manage.py startapp polls

Writing views
from django.http import HTTPResponse
views.py 

Mapping views to url using include and path
from django.urls import path
urls.py

Part 2
Database setup
settings.py

Create tables from the installed apps
python manage.py migrate

Creating your own models - create classes and define fields
from django.db import models
models.py

Activating Models
Updating the Installed Apps on settings.py with your model
polls.app.PollsConfig

Let Python know you made some changes
python manage.py makemigration polls

Finally again run
python manage.py migrate




