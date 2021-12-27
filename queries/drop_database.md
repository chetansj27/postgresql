## Drop Database

```sql

DROP DATABASE IF EXISTS dbname;

```

If you are connected to database, it can give error **database used by other user**
```sql

SELECT
	pg_terminate_backend (pg_stat_activity.pid)
FROM
	pg_stat_activity
WHERE
	pg_stat_activity.datname = 'dbname';
```  
above query will terminate the session
