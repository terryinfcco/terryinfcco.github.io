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
# You have to specifically ask for the rowid 
# WHERE lets you search, can also use < = > >= <= for numerics
# LIKE lets you do fuzzy searches, % is wildcard rather than *
c.execute("SELECT rowid, * FROM customers WHERE last_name = 'Elder'")
c.execute("SELECT rowid, * FROM customers WHERE last_name LIKE 'Br%'")
c.execute("SELECT rowid, * FROM customers WHERE email LIKE '%codemy.com'")
# This is returned as a python list of tuples I think
items = c.fetchall()

# Now have to commit the changes every time you make changes
conn.commit()
# Close the connection when you're done
conn.close()
```