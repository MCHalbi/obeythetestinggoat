# Obey the testing goat – Cheatsheet
## Prerequisites
### Virtual environment ([» Full description](http://www.obeythetestinggoat.com/book/pre-requisite-installations.html#_setting_up_your_virtualenv))
_Setting up virtual environment with python 3.7:_
```
$ python3.7 -m venv virtualenv
```

_Activate virtual environment:_
```
$ sourec virtualenv/bin/activate
```

_Deactivate virtual environment:_
```
(virtualenv)$ deactivate
```

### Installing Django 1.11 and Selenium ([» Full description](http://www.obeythetestinggoat.com/book/pre-requisite-installations.html#_installing_django_and_selenium))
```
(virtualenv)$ pip install "django<1.12" "selenium<4"
```

## Django
### Creating a new project
_Create new Django project:_
```
$ django-admin.py startproject <project-name> .
```
This will create the following project structure:
```
.
├── manage.py
└── <project-name>
    ├── __init__.py
    ├── settings.py
    ├── urls.py
    └── wsgi.py
```

### Running dev server
```
$ python manage.py runserver
```
This will start a dev server at `http://127.0.0.1:8000`.

### Creating a new app
_Create new Django app in a project:_
```
$ python manage.py startapp <app-name>
```
This will create the following project structure:
```
.
├── <app-name>
│   ├── admin.py
│   ├── apps.py
│   ├── __init__.py
│   ├── migrations
│   │   └── __init__.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
├── manage.py
└── <project-name>
    ├── __init__.py
    ├── __pycache__
    ├── settings.py
    ├── urls.py
    └── wsgi.py
```

### Django test runner
```
$ python manage.py test
```
