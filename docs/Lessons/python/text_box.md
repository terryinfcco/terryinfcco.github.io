## Text Box

    from guizero import App, Text
    app = App(title = "Hello World")
    
    # Now put a line of text in window "app"
    message = Text(app, text = "Welcome to the app")
    
    app.display()
    
Properties:

    # Change Text Size:
    message.text_size = 50
    # Change Font
    message.font = "Times New Roman"
    # Change Text Color
    message.text_color = "white"