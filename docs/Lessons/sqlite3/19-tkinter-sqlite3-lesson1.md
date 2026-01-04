## Codemy.com tkinter lesson 19

### Steps
- Create a new database or connect to an existing one.
- Create a cursor which is needed to interact with the database
- sqlite3 only has 5 datatypes.
	- text
	- integer
	- real
	- null
	- blob
- Create the table 
``` python
import sqlite3
# Create a database or connect to one
# Same command does both
conn = sqlite3.connect('address_book.db')

# Have to create a cursor to interact with the database
c = conn.cursor()

# Create a table within the database
c.execute("""CREATE TABLE addresses (
	first_name text,
	last_name text, 
	address text,
	city text,
	state text,
	zipcode integer
	)""")


# Anytime we change the database, commit it.
conn.commit()

# Finally close the connection to make sure things get cleaned up.
conn.close()
```