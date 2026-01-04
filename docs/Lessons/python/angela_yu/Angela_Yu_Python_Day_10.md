## Functions with Outputs
- Use the `return` statement to return the output of the function

``` python
def format_name(f_name, l_name):
	formatted_f_name = f_name.title()
	return f"{formatted_f_name} {formatted_l_name}

formatted_string = format_name(f_name:"angela", l_name:"ANGELA")
print(formatted_string)

# Or could:
print(format_name(f_name:"AnGela", l_name:"YU"))
```

## Functions with Multiple Return Values

- `return` statement ends a function - anything after that doesn't get executed
- You can have multiple return statements in a function.

``` python
def format_name(f_name, l_name):
	if f_name == "" or l_name == "": # if no inputs, just quit
		return "You did not provide valid inputs"
	formatted_f_name = f_name.title()
	return f"{formatted_f_name} {formatted_l_name}

formatted_string = format_name(f_name:"angela", l_name:"ANGELA")
print(formatted_string)

# Or could:
print(format_name(f_name:"AnGela", l_name:"YU"))
```

## Docstrings
- Little bits of documentation included in our code
- Goes immediately after def statement
- Enclosed in triple double quotes.
- Shows in documentation for the function
- Docstrings that aren't immediately after a def statement are just multiline comments, but the python documentation recommends against using docstrings for multiline comments. Just start each line with # 
- 
``` python
""" Take a first and last name and format it to 
return the title case version """

```