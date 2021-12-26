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
