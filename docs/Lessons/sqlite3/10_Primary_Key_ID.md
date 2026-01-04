- Primary Key is a unique ID number that each row of the database gets
- SQLite automatically creates a primary key called rowid for each record

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
c.execute("SELECT rowid, * FROM customers")
# This is returned as a python list of tuples I think
items = c.fetchall()

# Now have to commit the changes every time you make changes
conn.commit()
# Close the connection when you're done
conn.close()
```