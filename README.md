# django-howto
Django Howtos tutorial

Notes Covered: MySite
Part 1
Creating a django project
 django-admin startproject mysite

Run the server
``` ssh
 python manage.py runserver
```

Creating an app
``` ssh
 python manage.py startapp polls
```

Writing views - views.py
``` ssh
from django.http import HTTPResponse
```

Mapping views to url using include and path - urls.py
``` ssh
from django.urls import path
```

Part 2
Database setup - settings.py

Create tables from the installed apps
``` ssh
python manage.py migrate
```

Creating your own models - create classes and define fields - models.py
``` ssh
from django.db import models
```

Activating Models
Updating the Installed Apps on settings.py with your model
polls.app.PollsConfig

Let Python know you made some changes
``` ssh
python manage.py makemigration polls
```

Finally again run
``` ssh
python manage.py migrate
```



