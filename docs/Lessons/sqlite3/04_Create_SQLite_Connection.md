---
tags:
  - sqlite3
  - python
---
# 04 Create SQLite3 Connection

``` python title="Create Connection to DB "
# Have to import the sqlite3 module
import sqlite3
# Create a connection to the database
# If the database doesn't exist it will create it.
conn = sqlite3.connect('customer.db')
```
- Possible to create database in memory
- Disappears when program end.
`conn = sqlite3.connect(':memory:')`
