---
tags: [Functions Python]
---

## Python Functions

Define your own functions. def func_name(arg1, arg2): then indent the body of the function. Functions can return values.

```python
def combine_name(first_name, last_name):
	full_name = first_name + " " + last_name
	print(full_name)
combine_name("Terry", "Dutcher")

```

Can return values from a function.

```python

def combine_name(first_name, last_name):
	full_name = first_name + " " + last_name
	return full_name

fname = combine_name(first_name, last_name)
print (fname)

```
