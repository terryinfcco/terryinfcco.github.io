---
tags:
    - Dave_Gray
    - Django
---

# 1d Django HTML Templates


## Start Using Templates for Real HTML Pages

- Create `templates` folder alongside lower myproject and manage.py
- Create `templates/home.html` and `templates/about.html`
- Use emmet ! to create a template and on the home page an h1 and a link to the about page.
- Same general thing for about page.
- In settings.py go to the TEMPLATES section and change `'DIRS': [],` to
`'DIRS': ['templates'],
- Now change views.py to use our templates.
