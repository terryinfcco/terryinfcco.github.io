## Push Button

	from guizero import PushButton
	
    # Create a button in container app,
    # function to run is choose_name
    # button text is Tell me!
    	
	button = PushButton(app, choose_name, text="Tell me!")
	
	# Change the button background color
	button.bg = "red"
	# Change the button text size
	button.text_size = 20
	# Change the button font
	button.font = "Times New Roman"
	# Change the button text_color
	button.text_color = "white"
	
	app.display()
	