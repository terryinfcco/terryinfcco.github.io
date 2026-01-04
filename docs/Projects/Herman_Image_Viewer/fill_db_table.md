---
tags:
  - python
  - sqlite3
  - HermanImageViewer
---
# Initial Fill of Database for Herman Image View Project

``` python title="Program to fill the database initially"
import sqlite3
import glob

# grab all the images from the right subdirectory
image_list = glob.glob("/home/terry/Nextcloud/herman/*.png")

# Create a connection
conn = sqlite3.connect('herman.db')
# Create a cursor
c = conn.cursor()

# Now loop through the image list adding each image to the images table in herman.db
for image in image_list:
    print("Inserting: ", image)
    c.execute("""INSERT INTO images(full_filename,view_count) VALUES (?,?)""", (image, 0))

c.execute("SELECT rowid, * FROM images")
print(c.fetchall())
conn.commit()
conn.close()
```
