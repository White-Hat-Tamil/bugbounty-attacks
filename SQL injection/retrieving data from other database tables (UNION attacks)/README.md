# If sqli query result returned in application response, we can use UNION to retrieve data from other tables within database

SELECT a, b FROM table1 UNION SELECT c, d FROM table2
This SQL query returns a single result set with two columns, containing values from columns a and b in table1 and columns c and d in table2
