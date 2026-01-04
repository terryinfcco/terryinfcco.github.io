# Flask Mega Tutorial Video 1
- I created a folder called flask/miguel and changed to it.
- Make sure python is installed
- Install flask - he created a folder called microblog and put a venv called venv in it.
- Then a subdirectory called app and an `__init__.py` file.
- Not sure I understand the explanation but he says this kind of base ensures flask is correctly set up.
``` python title="__init__.py"
from flask import Flask 
app = Flask(__name__)
from app import routes
```
- And then he creates the program routes.py in the app subdirectory
``` python title="routes.py"
from app import app

@app.route('/')
@app.route('/index')
def index():
    return "Hello, World"
```
- And then in microblog, he creates microblog.py
``` python title="microblog.py"
from app import app
```
- Now to tell Flask what to run
``` bash
export FLASK_APP=microblog.py
```
- finally run the app
``` bash
flask run
```
- To avoid having to run the export command everytime you want to do this:
`pip install python-dotenv` (making sure the venv is active)
then at the top level directory of the project create `.flaskenv`
`FLASK_APP=microblog.py`

