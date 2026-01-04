---
tags:
    - Dave_Gray
    - Django
---

# 1c Simple Web Page
## URL's

- Each web page requires an entry in *urls.py* and in *views.py*
- Now edit myproject/myproject/urls.py and add the home page and about page urls. Will still need to add views. Every page has to have a URL and a View.
``` python
urlpatterns = [
    path('admin/', admin.site.urls),
    path('', ),
    path('about/',),
```

## Views
- create myproject/myproject/views.py
``` python
from django.http import HttpResponse

def homepage(request):
    return HttpResponse("Hello World! I'm Home.")
def about(request):
    return HttpResponse("My About page.")
```
## Finish URL's
- Go back to the urls.py file and add in the views we created. Have to import views file first
``` python
from . import views

urlpatterns = [
    path('admin/', admin.site.urls),
    path('', views.homepage),
    path('about/', views.about),
```
