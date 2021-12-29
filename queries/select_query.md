To retrieve data from all columns
```sql
SELECT * FROM table_name;
```
FROM clause is evaluated before SELECT<br><br>


To retrieve data from specific columns
```sql
SELECT column_name1,column_name12,... FROM table_name;
```


## Alias<br><br>
This query will return the data of first_name column in firstName column. AS keyword is optional<br>
```sql
SELECT first_name AS "First Name" FROM demo;
```
<br>

This query will combine the first_name and last_name column having a space between them and return into a column Full Name.<br>
```sql
SELECT 
	first_name || ' ' || last_name AS "Full Name" 
FROM demo;
```
