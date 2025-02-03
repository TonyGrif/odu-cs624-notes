# SQL
Structured Query Language is the standard language for storing, retrieving, and manipulating data found in [[Relational Databases | relational databases]].
## Standard Commands
While there are many variations on SQL commands based on the specific database, all support certain commands to remain ANSI compliant. SQL keywords are not case-sensitive while values are.
### SELECT
This command is used to retrieve data. This command takes the form of `SELECT {column(s)} from {table};` A `*` can be used for the column field to select all columns in the table. Columns are separated by a comma when querying multiple.
#### SELECT DISTINCT
This statement returns the distinct values from a column(s). This takes the form of `SELECT DISTINCT {column(s)} from {table};`.
### WHERE
This command is used to conditionally filter results. This takes the form of `COMMAND {column(s)} from {table} WHERE {condition};`. When conditionally checking a text data type, place quotes around the value; when conditionally checking a numeric data type, do not use quote.
#### Operators
| Operator | Condition                                     |
| -------- | --------------------------------------------- |
| =        | Equal                                         |
| >        | Greater Than                                  |
| <        | Less Than                                     |
| >=       | Greater Than or Equal                         |
| <=       | Less Than or Equal                            |
| != or <> | Not Equal                                     |
| BETWEEN  | Between a Range                               |
| LIKE     | Search for a Pattern                          |
| IN       | Specify Multiple Possible Values for a Column |
### ORDER BY
This command sorts the results of a query. This takes the form of `SELECT {column(s)} from {table} ORDER BY {column}`. By default, this will sort in ascending order; to sort in descending order, append `DESC` to the end of the `ORDER BY` command. Sorting can be done on multiple columns; this is works by placing `ORDER BY {col1}, {col2};` at the end of the query. This will sort the results by the first column; then, if the rows are the same, sort by the second column. 
## Logical Operators
These operators are used to determine logic between statements by manipulating boolean values.
### Available Operators
* AND
* OR
* NOT
### Chaining Operators
You can chain these operators together with a specific order of operations using parenthesis. Conditions within the parenthesis are evaluated first, before moving out to the rest of the statement.