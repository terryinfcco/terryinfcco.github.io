# Neural Nine Full Flask Course Routes and URL's

## Summary
Having multiple routes is just a matter of adding a decorator and function.
Variables can be included in the URL using `<>`

``` python title="app.py"
from flask import Flask

app = Flask(__name__)

@app.route('/')
def index():
    return "<h1>Hello World</h1>"

# Route doesn't have to match the name of the function
@app.route('/hello')
def hello():
    return "Hello World"

@app.route('/greet/<name>')
def greet(name):
    return f"Hello {name}"

if __name__ == '__main__':
    app.run(host='localhost', port=5555, debug=True)
```

