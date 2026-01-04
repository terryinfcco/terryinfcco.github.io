---
tags:
    - Python
    - Udemy
    - AngelaYu
---

# 100 Days of Python
### Udemy
### Angela Yu 
## Day 2 
### Data Types 
- String, Int, Float, Boolean 
- string[int] - Gets Nth char of a string, n starts at zero 
``` python
nth = user_name[3] # 4th character of the user_name
first_char = "Hello"[0] # 1st character of Hello
```
- In #'s you can put underscores where commas might go
- 1,234,567 can be entered as 1_234_567 
- Boolean True or False - always capitalized without quotes
- Can't concatenate int to string. 
``` python 
print("Your Name has "+ str(len(name)) + " characters") # convert to str
```
- type() function will give the type of what's in the parentheses
- python does lots of implicit conversions
``` python
print(70 + float("100.5")) # python converts 70 (an integer) to a float implicitly
```

### Math Operators 
- +, -, *, /, ** 
- division always results in float 
- rules for precedence in python in this order:
- parantheses, exponents, (multiply, divide done Left to Right), (+, - done Left to Right) 
``` python
a = 3 * 3 +3 / 3 - 3
print(a) # answer is 7.0 (9 + 1.0 - 3)
b = 3 * (3 + 3) / 3 - 3
print(b) # answer is 3.0 (3 * 6 / 3 - 3)
```

### Number Manipulation and F Strings
- round function can set number digits to round to, default is zero
``` python
print(round(8 / 3, 2)) # Round to 2 digits --> 2.67
```
- floor division (// rather than /) gives a truncated integer
``` python
print(8 // 3) # Gives integer answer of 2
```
``` python 
# math shorthand works for +, -, *, /
result /= 2 # Divide result by 2 
var += 1 # Add 1 to var
```
- f strings used mostly in printing but works other places
- character f in front of the string, variables in curly braces.
- Don't have to convert everything to strings this way.
``` python
print(f"Your score is {score}") 
```

#udemy
#angelayu
#python
