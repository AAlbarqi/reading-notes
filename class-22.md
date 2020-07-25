# SQL

###### Database Schema
the database schema is what describes the structure of each table, and the datatypes that each column of the table can contain.
###### SELECT queries 

To retrieve data from a SQL database, we need to write SELECT statements, which are often colloquially refered to as queries.

- Select query for a specific columns
`SELECT column, another_column, … FROM mytable;`

- Select query for all columns
`SELECT * FROM mytable;`

###### Queries with constraints

In order to filter certain results from being returned, we need to use a WHERE clause in the query. The clause is applied to each row of data by checking specific column values to determine whether it should be included in the results or not.

- Select query with constraints
`SELECT column, another_column, … FROM mytable WHERE condition AND/OR another_condition`

###### Filtering and sorting Query results
Even though the data in a database may be unique, the results of any particular query may not be – take our Movies table for example, many different movies can be released the same year. In such cases, SQL provides a convenient way to discard rows that have a duplicate column value by using the DISTINCT keyword.

- Select query with unique results
`SELECT DISTINCT column, another_column, … FROM mytable WHERE condition(s);`

###### Ordering results
SQL provides a way to sort your results by a given column in ascending or descending order using the ORDER BY clause.

- Select query with ordered results
`SELECT column, another_column, … FROM mytable WHERE condition(s) ORDER BY column ASC/DESC;`

###### Limiting results to a subset
Another clause which is commonly used with the ORDER BY clause are the LIMIT and OFFSET clauses, which are a useful optimization to indicate to the database the subset of the results you care about.
The LIMIT will reduce the number of rows to return, and the optional OFFSET will specify where to begin counting the number rows from.
- Select query with limited rows

`SELECT column, another_column, … FROM mytable WHERE condition(s)`
`ORDER BY column ASC/DESC LIMIT num_limit OFFSET num_offset;`

###### Inserting rows
- Insert statement with values for all columns

`INSERT INTO mytable (column, another_column, …) VALUES (value_or_expr, another_value_or_expr, …),`
       `(value_or_expr_2, another_value_or_expr_2, …), …;`

###### Updating rows

- Update statement with values
`UPDATE mytable SET column = value_or_expr,` 
`other_column = another_value_or_expr, WHERE condition;`

###### Deleting rows

- Delete statement with condition
`DELETE FROM mytable WHERE condition;`

###### Creating tables

- Create table statement w/ optional table constraint and default value
`CREATE TABLE IF NOT EXISTS mytable (`
    `column DataType TableConstraint DEFAULT default_value,`
    `another_column DataType TableConstraint DEFAULT default_value,);`

- Here's an example schema for the Movies table that we've been using in the lessons up to now.

`Movies table schema
CREATE TABLE movies (
    id INTEGER PRIMARY KEY,
    title TEXT,
    director TEXT,
    year INTEGER, 
    length_minutes INTEGER
);`

###### Altering tables
ALTER TABLE statement to add, remove, or modify columns and table constraints.

- Altering table to add new column(s)
`ALTER TABLE mytable ADD column DataType OptionalTableConstraint DEFAULT default_value;`

- Altering table to remove column(s)
`ALTER TABLE mytable DROP column_to_be_deleted;`

- Renaming the table, Altering table name
`ALTER TABLE mytable RENAME TO new_table_name;`

###### Dropping tables
you may want to remove an entire table including all of its data and metadata, and to do so, you can use the DROP TABLE statement, which differs from the DELETE statement in that it also removes the table schema from the database entirely.

- Drop table statement
`DROP TABLE IF EXISTS mytable;`


- [SQL Cheat Sheet](http://www.cheat-sheets.org/sites/sql.su/)