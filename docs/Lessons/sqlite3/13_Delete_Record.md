``` python
# Have to import the module
import sqlite3
# Create a connection to the database
# If the database doesn't exist it will create it.
conn = sqlite3.connect('customer.db')
# Always Have to create a cursor
c = conn.cursor()

# Delete Records remember rowid is an integer
c.execute("DELETE from customers WHERE rowid = 6)

# Now have to commit the changes every time you make changes
conn.commit()

# Query the Database - Sets up what records you want
# In this case we're selecting everything '*'
c.execute("SELECT rowid, * FROM customers")
# This is returned as a python list of tuples I think
items = c.fetchall()

for item in items:
	print(item)


# Close the connection when you're done
conn.close()
```
