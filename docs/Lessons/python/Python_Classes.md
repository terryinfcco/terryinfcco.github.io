## Python Classes

Fundamental to Object Oriented. A Class is the "blueprint" for an object. Python has lots of built in classes - like the methods .upper() or .lower() for a string. Functions inside a class are referred to as methods. The first method in any class is the __init__ method. Convention is that class names are capitalized.

```python
class Square:
	def __init__(self, side_length):
		self.side_length = side_length
	
	def area(self):
		return self.side_length * self.side_length

	def perimeter(self):
		return self.side_length * 4

	def report(self):
		print ("Side Length: %s" % self.side_length )
		print ("Area: %s" % self.area())
		print ("Perimeter: %s" % self.perimeter())

my_square = Square(5)
my_square.report()

```

#tagcheck
#tagcheck
