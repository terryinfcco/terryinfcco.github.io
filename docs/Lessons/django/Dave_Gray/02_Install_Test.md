---
tags:
    - Dave_Gray
    - Django
---

# 1b Django Install and Test

## Install Django in a Virtual Environment

``` shell
mkdir lesson01
cd lesson01
python -m venv .venv
source .venv/bin/activate 
pip install Django # He's on Django 5.0.1
pip install --upgrade pip # if needed
python # enter the interactive python shell
```

## Make Sure the Installation Worked

- Make sure Django is installed
``` python
import django
print(django.get_version())
quit()
```

## Create the Project

- Create project - pretty standard, he doesn't use the period so we have a sublevel myproject folder.
- Using port 8001 because I'm starting mkdocs on 8000
``` shell
django-admin startproject myproject # Creates myproject/myproject structure
cd myproject
python manage.py runserver 8001 # port 8001 default is 8000
```
## Make Sure it Worked


- Go to browser and check out `localhost:8001` # should see little rocket ship page
