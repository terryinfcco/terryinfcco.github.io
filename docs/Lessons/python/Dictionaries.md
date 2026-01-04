---
tags:
    - Python
    - Dictionaries
---

## Python Dictionaries

Made up of key / value pairs.  Created using curly braces. Values could be a list. And the key can be a number rather than a string.

```
fav_pizza = {
    "John": "Pepperoni",
    "Bob": "Mushroom",
    "Mary": "Cheese"
    }

print (fav_pizza["John"]) # will print Pepperoni
print (fav_pizza["Mary"]) # will print Cheese

del fav_pizza["John"] # John will be deleted from the dictionary

fav_pizza.update({"Tina": "Green Peppers"}) # Tina is added to dictionary

fav_pizza["John"] = "Green Peppers" # John changed to Green Peppers


```

