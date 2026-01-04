---
tags:
  - sqlite3
  - python
---
# 06 Insert One Record Into Table

``` python title="Insert Record into DB Table"
# Have to import the module
import sqlite3
# Create a connection to the database
# If the database doesn't exist it will create it.
conn = sqlite3.connect('customer.db')
# Always Have to create a cursor
c = conn.cursor()
# Now add a record to the database table customers
# Our fields are first_name, last_name, and email.
# Notice you have to nest single quotes in the double quotes
c.execute("INSERT INTO customers VALUES ('John', 'Elder', 'john@codemy.com')")
# Now have to commit the changes every time you make changes
conn.commit()
# Close the connection when you're done
conn.close()
```
