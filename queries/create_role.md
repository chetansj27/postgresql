

## Create role
```sql
CREATE ROLE chetan WITH LOGIN SUPERUSER CREATEDB CREATEROLE INHERIT REPLICATION CONNECTION LIMIT -1 VALID UNTIL '2025-01-05T12:36:23+05:30' PASSWORD 'xxxxxx';
```
This will create role chetan with all privileges and password is valid till 05 Jan 2025. 

Connection limit -1 means no limit.

Inherit means inherit privileges of roles it is a member of.

Replication means can copy data from one server to another.

CREATEDB means have access to create data

CREATEROLE means have access to create roles

LOGIN means user can login
 
