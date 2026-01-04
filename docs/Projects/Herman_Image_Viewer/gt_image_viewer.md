---
tags:
  - python
  - sqlite3
  - HermanImageViewer
---
# Actual Herman Image Viewer Program

``` python title="Herman Image Viewer"
import sqlite3
from tkinter import *
from PIL import ImageTk, Image

root = Tk()
root.title('Grandpa Terry Image Viewer')
# grab one image with a view_count of zero
conn = sqlite3.connect('herman.db')
c = conn.cursor()

c.execute("SELECT rowid, * from images WHERE view_count = 0")
image = c.fetchone()
# print(image)
# my_img = ImageTk.PhotoImage(Image.open("/home/terry/Nextcloud/herman/533strip.png"))
my_img = ImageTk.PhotoImage(Image.open(image[1]))
my_label = Label(image=my_img)
my_label.pack()

count = image[2] + 1
rownum = image[0]

# print("Count: ", count, "Rownum: ", rownum)

# Now that we've displayed the image increment it's view_count
c.execute("""UPDATE images SET view_count = (?) WHERE rowid = (?)""", (count, rownum))
conn.commit()

# Put a status bar with image name and how many pix total and left to view
# print("image[1]: ", image[1])
last_slash = image[1].rfind('/')
status_label = Label(text=image[1][last_slash + 1:])
status_label.pack()


conn.close()

button_quit = Button(root, text="Exit Program", command=root.quit)
button_quit.pack()
root.mainloop()
```
