#  DATABASE NORMALIZATION

## What is Database normalization ?

Database normalization is a process used to organize a database into tables and columns. 
The main idea with this is that a table should be about a specific topic and only supporting topics included.

* There are three common forms of database normalization: 1st, 2nd, and 3rd normal form.

1. **First Normal Form** – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
2. **Second Normal Form** – The table is in first normal form and all the columns depend on the table’s primary key.
3. **Third Normal Form** – the table is in second normal form and all of its columns are not transitively dependent on the primary key

## Reasons for Database Normalization

**1- By limiting a table to one purpose you reduce the number of duplicate data contained within your database.**
**2- This eliminates some issues stemming from database modifications.**
**3- to simplify queries.**

## Data Duplication and Modification Anomalies

Duplicated information presents two problems:

1. It increases storage and decrease performance.
2. It becomes more difficult to maintain data changes.

**There are three modification anomalies that can occur:**
1- Insert Anomaly
2- Update Anomaly
3- Search and Sort Issues


