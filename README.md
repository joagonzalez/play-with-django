# django-seed
![Python](https://img.shields.io/badge/django-v4.0.1-orange)
![Python](https://img.shields.io/badge/python-v3.8.10-blue)
![Python](https://img.shields.io/badge/platform-linux--64%7Cwin--64-lightgrey)

This repo works on some basic examples for building www sites within django framework.

- app1/: Example django project. Inside this folder you can find some apps, like *polls*, in which different features and capabilties of the framework will be tested
- examples/: Examples of some technologies like html, css and databases that will be used within django

### app1

```
workon django
cd app1/

# check for sintax or programming errors
django/app1(development)$ python manage.py check
System check identified no issues (0 silenced).

# run development server
django/app1$ python manage.py runserver
Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).
January 30, 2022 - 19:04:12
Django version 4.0.1, using settings 'app1.settings'
Starting development server at http://127.0.0.1:8000/

# run migration/updates for data models of the applications
django/app1(development)$ python manage.py migrate
Operations to perform:
  Apply all migrations: admin, auth, contenttypes, polls, sessions
Running migrations:
  No migrations to apply.

# create super user for django model administrator
django/app1(development)$ python manage.py createsuperuser

# start python shell with django context
django/app1(development)$ python manage.py shell
Python 3.8.10 (default, Nov 26 2021, 20:14:08) 
[GCC 9.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
(InteractiveConsole)
>>> 

# create a new app within project and directory/file structure
django/app1(development)$ python manage.py startapp something

django/app1(development)$ tree something/
something/
├── admin.py
├── apps.py
├── __init__.py
├── migrations
│   └── __init__.py
├── models.py
├── tests.py
└── views.py

1 directory, 7 files

# create a new project with initial directory/file structure
django/app1(development)$ django-admin startproject app1
```
