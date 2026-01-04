``` python title="Insert Many Records into DB Table"
# Have to import the module
import sqlite3
# Create a connection to the database
# If the database doesn't exist it will create it.
conn = sqlite3.connect('customer.db')
# Always Have to create a cursor
c = conn.cursor()
# Create a list to show how this works.
many_customers = [('Wes', 'Brown', 'wes@brown.com'), 
		('Steph', 'Kuewa', 'steph@kuewa.com'),
		('Dan', 'Pas', 'dan@pas.com'),
	 ]
# Now add the list to the database
# You use question marks as placeholders for what you're inserting
c.executemany("INSERT INTO customers VALUES (?,?,?)", many_customers)
# Now have to commit the changes every time you make changes
conn.commit()
# Close the connection when you're done
conn.close()
```
