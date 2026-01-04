Text Widget

``` python
from guizero import App, Text
app = App(title="Hello World")
message = Text(app, text="Welcome to the app")
app.display()
```

## Change Font and Size

``` python
message.font = "Times New Roman"
message.text_size = 50
```


