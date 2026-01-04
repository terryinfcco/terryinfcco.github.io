# Neural Nine Full Flask Course Basics

## Summary
Basic setup of a flask app, and creation of the index or home route.
## Specifics
- He created a directory called firstapp
- He created a virtual environment called `.venv` and activated it.
- `pip install flask`
- Creates `app.py`

``` python title="app.py"
from flask import Flask

app = Flask(__name__)

@app.route('/')
def index():
    return "Hello World"

if __name__ == '__main__':
    app.run(host='localhost', debug=True)
```


