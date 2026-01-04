## Python String Formatting

F-Strings (python 3.6+) used by python to interpolate values.

```
guess = 8
print (f"your guess of {guess} was incorrect!")

name = "bluethecat"
print(f"Nice try, {name} but your guess of {guess} is wrong!")
```

Old ways:

```
x = 10
formatted = "I've told you {} times already!".format(x)

x = 10
formatted = "I've told you %d times already!" % (x)
```
