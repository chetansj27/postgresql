```sql
INSERT INTO upsertdemo(t_name) 
VALUES('chetan')
ON CONFLICT(t_name)
DO NOTHING;
```
Above query will insert data in upsertdemo table in t_name(which has unique constarint)cloumn. If the value is already present in t_name column means conflict column it will not perform any action.


```sql
INSERT INTO upsertdemo(t_name) 
VALUES('chetan')
ON CONFLICT(t_name)
DO
UPDATE SET
	t_name=EXCLUDED.t_name,
	update_date=NOW();
```
Above query will insert data in upsertdemo table in t_name(which has unique constarint)cloumn. If the value is already present in t_name column means conflict column it will update the value.

