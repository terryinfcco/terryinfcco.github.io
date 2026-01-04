## Python Strings

----

**Single and Double Quotes**

Can use either single or double quotes, but you need to be consistent within the same line. Good style says you should be consistent within your program.

if you want to use one or the other in the string you have to use the opposite one to delineate the string:

```
print ("I can't do this with all single quotes")
```

**Escape Sequences**

All start with backslashes. e.g. \n - newline, \\ - backslash, \' - single quote, \" - double quote.

Strings are indexed.

    a = "hello"
    a[0] ==> h
    a[4] ==> o

reverse indexing:

    a[-1] ==> o
    a[-4] ==> e

slices:

    a[0:2] ==> he  --note that the result goes up to but doesn't include the final index
    alpha = 'abcdef'
    a[2:4] ==> cd
    a[2:] ==> cdef

methods:
 change the variable itself. Some change the variable, others have to be assigned to a variable
 
    basic = "Hello World"
    upper_basic = basic.upper()  ==> HELLO WORLD
    basic.split() ==> returns list of all words separated by spaces
    basic.split('a') ==> splits on a's not on spaces.
 
formatted printing:

    user_name = 'Recruit'
    action = 'run'
    print('The {} needs to {}'.format(user_name,action)) ==> The Recruit needs to run
 
----

