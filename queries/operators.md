## Operators

### AND operator

Below query will return rows where movie_lang='English'AND age_certificate='18'
```sql
SELECT * FROM movies WHERE 
movie_lang='English' AND age_certificate='18';
```
<br>

### OR operator

Below query will return rows where movie_lang='English'or age_certificate='18'
```sql
SELECT * FROM movies WHERE 
movie_lang='English' OR age_certificate='18';
```
<br>

### Combining AND OR operator

Below query will return rows where movie_lang is either English or Chinese and age_certificate is 15.
```sql
SELECT * FROM movies 
WHERE 
	(movie_lang='English' OR movie_lang='Chinese')
	AND age_certificate='15';
```



