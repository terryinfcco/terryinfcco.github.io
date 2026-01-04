---
tags:
  - python
  - sqlite3
  - HermanImageViewer
---

# Program to Create The Database and Table for the Herman Image Viewer Project

``` python title="Program to Create Herman Database and Images Table"
import sqlite3

# Create a connection
conn = sqlite3.connect('herman.db')
# Create a cursor
c = conn.cursor()

# The table is just the filename of the image and a count of the number of times that particular image has been viewed
c.execute("""CREATE TABLE images(
    full_filename DATATYPE text,
    view_count DATATYPE integer)
""")

# commit the change
conn.commit()
# close the database
conn.close()
```