To insert data into table

```sql 
 INSERT INTO tablename(columnname1,columnname2,...) VALUES('value1','value2',...);
 ```
 
 To insert multiple rows:
 ```sql 
 INSERT INTO tablename(columnname1,columnname2,...) 
 VALUES
 ('value1','value2',...),
 ('value1','value2',...)
 ('value1','value2',...);
 ```
 
 To insert data which has quote(wrap the value with extra quote)
 ```sql
 INSERT INTO demo(first_name,last_name) VALUES('bill''o','sel');
 ```
 
 To see the inserted data
 ```sql
 INSERT INTO demo(first_name) VALUES('adam') RETURNING *;
 ```
 Above query will return all columns for inserted value
 
 
 ```sql
 INSERT INTO demo(first_name) VALUES('adam') RETURNING demo_id;
```
Above query will return specific column for inserted value
