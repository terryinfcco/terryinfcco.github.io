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
# c.fetchone()
# c.fetchmany(3) # grab 3 records
# c.fetchall()
# This is returned as a python list of tuples I think
print(c.fetchall())

# Now have to commit the changes every time you make changes
conn.commit()
# Close the connection when you're done
conn.close()
```

