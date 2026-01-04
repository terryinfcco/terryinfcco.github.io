---
tags:
    - Dave_Gray
    - Django
---
# 1e Static Files and CSS
- Put a `static` folder at the same level as the templates folder. And a folder in there called css.
- Create a file `style.css` in the css folder.

``` css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box:
}

body {
    min-height: 100vh;
    display: grid;
    place-content: center;
    font-size: 3rem;
    background-color: black;
    color: whitesmoke;
}

h1, p {
    text-align: center;
}
```
- in `myproject/myproject/settings.py`
``` python
import os # goes at top of file.
# Then after STATIC_URL = 'static/'
STATICFILES_DIRS = [
    os.path.join(BASE_DIR, 'static')
]
```
- Then in `home.html` after `<!DOCTYPE html>`
``` python
{% load static %}
```
- In `<head>` section after the title:
``` html
<link rel="stylesheet" href="{% static 'css/style.css' %}">
```
