``` python
# Have to import the module
import sqlite3
# Create a connection to the database
# If the database doesn't exist it will create it.
conn = sqlite3.connect('customer.db')
# Always Have to create a cursor
c = conn.cursor()

# Query the Database - Sets up what records you want
# In this case we're selecting everything '*'
# LIMIT allows you to only get a certain number of results.
c.execute("SELECT rowid, * FROM customers LIMIT 2")
# LIMIT has to go at end
c.execute("SELECT rowid, * FROM customers ORDER BY rowid DESC LIMIT 2")

# This is returned as a python list of tuples I think
items = c.fetchall()

for item in items:
	print(item)


# Now have to commit the changes every time you make changes
conn.commit()
# Close the connection when you're done
conn.close()
```