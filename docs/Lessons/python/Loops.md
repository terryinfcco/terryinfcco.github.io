## Python Loops

While loops are like if statements, you do something while a condition is true

```python
counter = 0
while (counter < 10):
	print ("The count is: %s" % counter)
	counter +=1
```

For Loops loop through something like a string, a list, or a dictionary.

```python
name = "John"
for x in name:
	print (x)  # prints J then o then h then n

fav_pizza = {
	"John": "Pepperoni",
	"Bob": "Cheese",
	"Tina": "Supreme"
}

for key, value in fav_pizza.items():
	print(key, value) # will go through the dictionary using the items function. Variables could be anything like name, style.
```
