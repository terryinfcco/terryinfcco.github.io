## Python Lists

List items are always created using square brackets:

```python
names = ["John", "Bob", "Mary"]
```

List items are indexed and always start with zero.
So:

```python
print(names[0]) # prints John
print(names) # prints all items in list.
```

Lists can contain more that one datatype.

Change one item in a list by addressing it directly:

```Python
names[0] = "Wes"
```

Append an item to a list:

```python
names.append("Wes") # Wes becomes 4th item in list.
```

Lists can contain other lists:

```python
nums = [1,2,3,4,5]
names = ["John", "Bob", "Tina", nums]
print(names[3,2]) prints 3
print(names[3,2] + 10) prints 13
```
```python
len(names) # returns number of items in the list.
```

