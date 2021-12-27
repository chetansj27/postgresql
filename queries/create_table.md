## Create Table

```sql
CREATE TABLE actor(
	actor_id SERIAL PRIMARY KEY,
	first_name VARCHAR(100) NOT NULL,
	last_name VARCHAR(100),
	gender CHAR(1),
	date_of_birth DATE,
	created_by VARCHAR(100),
	update_at DATE,
	created_at DATE
);
```
This will create foreign key of director_id.

```sql

CREATE TABLE movies(
	movie_id SERIAL PRIMARY KEY,
	movie_name VARCHAR(100) NOT NULL,
	movie_length INT,
	movie_language VARCHAR(20),
	movie_certificate VARCHAR(10),
	release_date DATE,
	director_id INT REFERENCES table_name(column_name)
);
```

Below query will create a junction table movies_actors which have movie_id and actor_id as foreign key from movies and actors table.
```sql
CREATE TABLE movies_actors (
	movie_id INT REFERENCES movies (movie_id),
	actor_id INT REFERENCES actors (actor_id),
	PRIMARY KEY (movie_id, actor_id)
);
```
