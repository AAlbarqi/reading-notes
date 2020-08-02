# DATABASE NORMALIZATION

Database normalization is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included.

**The database table** is where all the data in a database is stored, and without tables, there would not be much use for relational databases.
A database consists of one or more tables.  Each table is made up of rows and columns.  If you think of a table as a grid, the column go from left to right across the grid and each entry of data is listed down as a row.

### Reasons for Database Normalization
1. minimize duplicate data.
2. minimize or avoid data modification issues.
3. simplify queries. 


### There are three modification anomalies that can occur:

1. Insert Anomaly: There are facts we cannot record until we know information for the entire row. 
2. Update Anomaly: In this case we have the same information in several rows. For instance if the office number changes, then there are multiple updates that need to be made.  If we don’t update all rows, then inconsistencies appear.
3. Deletion Anomaly: Deletion of a row causes removal of more than one set of facts.

### Forms of database normalization:

There are three common forms of database normalization: 1st, 2nd, and 3rd normal form. They are also abbreviated as 1NF, 2NF, and 3NF respectively. 
The forms are progressive, meaning that to qualify for 3rd normal form a table must first satisfy the rules for 2nd normal form, and 2nd normal form must adhere to those for 1st normal form.

1. First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
2. Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
3. Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key