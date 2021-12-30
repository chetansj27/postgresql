## ORDER BY clause is used to sort the result.

By default it sort in ascending order.<br>

Below query will sort the movies table on basis of release_date in ascending order.

```sql
SELECT * FROM movies ORDER BY release_date;
```
<br>
Below query will sort the movies table on basis of release_date in ascending order.

```sql
SELECT * FROM movies ORDER BY release_date ASC;
```
<br>

Below query will sort the movies table on basis of release_date in descending order.

```sql
SELECT * FROM movies ORDER BY release_date DESC;
```
<br>

Below query will sort movies table on basis of release_date in desc and movie_name in asce. release_date order will be executed first.

```sql
SELECT * FROM movies 
ORDER BY 
release_date DESC,
movie_name ASC;
```
<br>

Order By on alias

```sql
SELECT 
	first_name,
	last_name AS surname
FROM actors
ORDER BY surname;
```
<br>

Below query will sort the table on basis of length of first_name.

```sql
SELECT 
	first_name,
	LENGTH(first_name) AS len
FROM actors
ORDER BY len DESC;
```
<br>

This query will sort the table on first_name and all null values will be at last.
```sql
SELECT first_name FROM actors
ORDER BY first_name DESC NULLS LAST;
```
<br>

## Distinct
This query will return distinct first_name
```sql
SELECT DISTINCT first_name FROM actors;
```
