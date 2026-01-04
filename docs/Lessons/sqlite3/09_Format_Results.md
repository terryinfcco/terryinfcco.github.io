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
c.execute("SELECT * FROM customers")
# At this point 3 options:
# c.fetchone() # Grabs first record from the Query
# c.fetchmany(3) # grab first 3 records from the Query
# c.fetchall()
# This is returned as a python list of tuples I think
# print(c.fetchall())
# This time put the list in a variable and loop through and print it.
items = c.fetchall()

for item in items:
	print(item[0] + " " + item[1] + " " + item[2] )
# Now have to commit the changes every time you make changes
conn.commit()
# Close the connection when you're done
conn.close()
```

