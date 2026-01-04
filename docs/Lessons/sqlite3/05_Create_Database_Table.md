---
tags:
  - sqlite3
  - python
---
# 05 Create Database Table
- Tables are the main part of a database
- Think of them like a spreadsheet - rows and columns
``` python title="Create DB Table"
# Have to import the module
import sqlite3
# Create a connection to the database
# If the database doesn't exist it will create it.
conn = sqlite3.connect('customer.db')
# Have to create a cursor to communicate with the database
c = conn.cursor()
# Use the cursor to create a table
# Using a docstring is recommended in the python documentation
# When doing a simple one line command probably just use regular quotation marks.
# SQLite3 commands are case sensitive
# SQLite3 DATATYPEs null, integer, real, text, blob (stored asis - used
# for images, etc.)
c.execute("""CREATE TABLE customers(
	first_name DATATYPE text,
	last_name DATATYPE text,
	email DATATYPE text
)""")
# Now have to commit the changes every time you make changes
conn.commit()
# Close the connection when you're done
conn.close()
```
