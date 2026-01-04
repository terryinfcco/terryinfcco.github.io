## 1. Python Class and Object
- Example of a blueprint that can be used to build multiple houses, but different colors
	- Once the house exists the connection to the blueprint disappears
- Python statement `a = 2` creates an integer object from the integer class
	- object has certain properties from the class - an ID, type: class 'int', value 2
	- but once created no longer bound to the class
	- `b = 3` creates another integer object, but the ID is different, the value is different, but the type is the same.
	- if `a = 2 and b = 2` python doesn't create 2 objects, just puts two labels on the same object
	- floats and strings are similar - they have an ID, a type, and a value
## 2. Python Class and Object Relationship
- A class is a template that defines an object / instance
	- Class has a name, attributes and behaviors
	- e.g. name: vehicle, attributes: color, behaviors: drive
- Every object / instance has a unique identifier used by Python internally
- Behaviors in a python instance are called methods
- Once the instance is created we have instance attributes and instance methods
- An object oriented program is a community of communicating objects
	- This communication is achieved using messages
	- python syntax for these messages is: `instance_name.message`
	- Called dot notation
## 3. Python Variable versus a Python Object
- Variable contains the address of the object called the object reference - it isn't the object itself
- But in the vast majority of cases you can think of the variable and the object as being the same
## 4. Python Object Reference
``` python
first_number = 2
number_copy = first_number
```
- A second object reference is created that points to the same object as first_number
- There's only one object in this case
## 5. Python an Immutable Object
- Once the object is created it cannot be changed
- If you change the value of the variable, a new object is created and the pointer in the variable object reference is changed to point there.
- Python has a garbage collection process that regularly gets rid of the objects that are no longer pointed to by a variable

