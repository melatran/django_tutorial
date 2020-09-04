# Django and Python Tutorial

[Tutorial](https://tutorial.djangogirls.org/en/installation/#pythonanywhere)

- Django is written in Python. We need Python to do anything in Django
- using pythonanywhere to host our blog and generate our api token
- similar to rails, don't move around structures of the directories and files
- remember to run everything in virtual env

## Virtual Environment
- virtualenv will isolate your python/django setup on a per project basis
- this means that any changes you make on one website won't affect any others you're also developing
- find the directory and create virtualenv

Option 1: `pipenv shell`

Option 2: `python3 -m venv myvenv`

## Installing Django
There should be a virutalenv prefix

`python -m pip install --upgrade pip`

**Setup packages with requirements**

```
touch requirements.txt

Django~=2.2.4

pip install -r requirements.txt
```

## Python
- exploring on python console
- to exit type `exit()` or `Ctrl + D`
- 2 ** 3 is the same as 2^3
- uppercase `"momo".upper()`
- to find the length `len("MoMo")`
- functions belong to objects like upper(); functions are methods
- othertimes, functions don't belong to anything like len() so "momo" was the parameter to the len function
- files will end with `.py`
- command `python filename.py`

## Django(framework written in Python)
**Framework:** set of components that help you develop websites faster and easier; similar to rails
- when a request comes to a web server, it's passed to Django which tries to figure out what is actually requested
- 'urlresolver' takes a list of patterns and tries to match the URL; Django checks patterns from top to bottom and it something matches, then Django passes the request to the associated function(view)

*metaphor* Mail carrier walks down the street and checks each house number against the one of the letter. If it matches, she puts the letter there (urlresolver)

- `view` look at db for info
- `django-admin startproject mysite .` builds the skeleton of the django project
- get the server running on http://127.0.0.1:8000/

```
//settings.py

STATIC_ROOT = BASE_DIR, 'static'
ALLOWED_HOSTS = ['127.0.0.1', '']
```

![install_worked](https://user-images.githubusercontent.com/59414750/92280536-d5ffef80-eeb6-11ea-9ece-6d08117350e2.png)

## Django Models