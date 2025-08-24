# If sqli query result returned in application response, we can use UNION to retrieve data from other tables within database

SELECT a, b FROM table1 UNION SELECT c, d FROM table2
<br><br>
This SQL query returns a single result set with two columns, containing values from columns a and b in table1 and columns c and d in table2
<br><br>
For a UNION query to work, two key requirements must be met:
<br>
The individual queries must return the same number of columns.
<br>
The data types in each column must be compatible between the individual queries.
<br>
To carry out a SQL injection UNION attack, make sure that your attack meets these two requirements. This normally involves finding out:
<br><br>
How many columns are being returned from the original query.
<br>
Which columns returned from the original query are of a suitable data type to hold the results from the injected query
