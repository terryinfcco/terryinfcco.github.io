
# Object oriented Python Chapter 2

To model a real world object in python, we need to decide what attributes the object has and what operations it will perform.

Think of a class as a template from which an object is created.

Code of a light switch written as a class. This class contains a single attribute and three methods.

```
# OO_LightSwitch
class LightSwitch():
    def __init__(self):
            # initialization code goes in the __init__ method. A method always has at least one parameter which by convention is named self.
            # Most other OOP languages call this initialization method a constructor.
            self.switchIsOn = False
    def turnOn(self):
            # turn the switch on
            self.switchIsOn = True
    def turnOff(self):
            # turn the switch off
            self.switchIsOn = False

# Create an instance of the LightSwitch class
# using o to start the variable name of an object or instance is a way to remember that this variable is an object.
oLightSwitch = LightSwitch()

```

In a method any variable that does not start with self is a local variable and goes away when the method exits.
Variables that begin with self are instance variables. These are usually initialized in the __init__ method.
All instances of an object get their own copy of the instance variables (self.switchIsOn) in the LightSwitch class.
Code of a class can be in the same program as the main program or you can put it in a separate file and import it into the main program.

```
# File: OO_LightSwitch_with_Test_Code.py
# OO_LightSwitch
class LightSwitch():
    def __init__(self):
        self.switchIsOn = False
    def turnOn(self):
        # turn the switch on
        self.switchIsOn = True
    def turnOff(self):
        # turn the switch off
        self.switchIsOn = False
    def show(self):
      # added for testing
      print(self.switchIsOn)

# Main code
oLightSwitch = LightSwitch()
# create a LightSwitch object
# Calls to methods
oLightSwitch.show()
oLightSwitch.turnOn()
oLightSwitch.show()
oLightSwitch.turnOff()
oLightSwitch.show()
oLightSwitch.turnOn()
oLightSwitch.show()

```

You can instantiate as many objects as you want from a single class.
`oLightSwitch2 = LightSwitch()`


## Building a Slightly More Complicated Class.
#tagcheck
#tagcheck
