## Dictionaries and Nesting
### Dictionaries
- Dictionary is a key:value pair.
- In Python `{Key: Value}` --> `{"Bug": "An error in a program."}`
- Keys can be numbers as well as strings
- For multiple entries in a dictionary:
``` python
programming_dictionary = {
"Bug": "An error in a program",
"Function": "A piece of code that can be called over and over",
}
```
- To access items in a dictionary:
``` python
print(programming_dictionary["Bug"])
```
- To add an item to a dictionary:
``` python
programming_dictionary["Loop"] = "The action of doing something over."
```
- To create an empty dictionary
`empty_dictionary = {}`
- Wiping an entire dictionary
`programming_dictionary = {}`
- Edit an item in a dictionary
`programming_dictionary["Bug"] = "Edited value for Bug"`
- Looping through a dictionary
``` python
for key in programming_dictionary:
    print(key) # Just prints the key
    print(programming_dictionary[key]) # prints the values
```
### Nesting
- Values in dictionaries can be lists or other dictionaries
``` Python
travel_log = {
    "France": ["Paris", "Lille", "Dijon"],
    "Germany": ["Stuttgart", "Berlin"],
}
print(travel_log["France"][1]) # Will print Lille
```

``` python
nested_list = ["A", "B", ["C", "D"]]
print(nested_list[2][1]) # Will print D
```
- Nested Dictionary
``` python
travel_log = {
    "France": {
        "cities_visited": ["Paris", "Lille", "Dijon"],
        "total_visits": 12
    },
    "Germany": {
        "cities_visited": ["Berlin", "Hamburg", "Stuttgart"],
        "total_visits": 5
    },
}

print(travel_log["Germany"]["cities_visited"][2]) # Will print Stuttgart
```


