To update single column
```sql
UPDATE demo 
SET last_name='bob'
WHERE demo_id=3;
```
Above query will update the last name cloumn where demo_id is 3 from demo table. 


To update multiple columns
```sql
UPDATE demo 
SET 
last_name='bill',
age=21,
first_name='adam'
WHERE demo_id=5;
```
