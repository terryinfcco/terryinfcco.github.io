``` python
# Have to import the module
import sqlite3
# Create a connection to the database
# If the database doesn't exist it will create it.
conn = sqlite3.connect('customer.db')
# Always Have to create a cursor
c = conn.cursor()

# Update a record using a docstring
c.execute("""UPDATE customers SET first_name = 'Bob'
			WHERE last_name = 'Elder'
""")
# Not best way to do it. Best way is to use rowid
c.execute(""" UPDATE customers SET first_name = 'John'
			WHERE rowid = 1
""")
# Now have to commit the changes every time you make changes
conn.commit()

# Query the Database - Sets up what records you want
# In this case we're selecting everything '*'
c.execute("SELECT * FROM customers")
# This is returned as a python list of tuples I think
items = c.fetchall()

for item in items:
	print(item)


# Close the connection when you're done
conn.close()
```