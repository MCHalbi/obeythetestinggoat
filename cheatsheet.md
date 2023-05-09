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
### Create new project
_Create new Django project:_
```
$ django-admin.py startproject <project-name> .
```
This will create a new Django project:
```
├── manage.py
└── <project-name>
    ├── __init__.py
    ├── settings.py
    ├── urls.py
    └── wsgi.py
```
