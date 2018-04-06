---
layout: default
---
- View All Users 
```sh
select Host, User from mysql.user;
```
- Create, Grant, Drop Users
```sh
CREATE USER 'username'@'%' IDENTIFIED BY 'password';
GRANT ALL ON database.* TO 'username'@'%';
DROP USER 'username'@'%';
```
- View database size 
```sh
SELECT table_schema "Data Base Name", SUM( data_length + index_length) / 1024 / 1024 "Data Base Size in MB" FROM information_schema.TABLES GROUP BY table_schema;
```
- View Table Sizes 
```sh
SELECT TABLE_NAME, table_rows, data_length, index_length, round(((data_length + index_length) / 1024 / 1024),2) "Size in MB" FROM information_schema.TABLES WHERE table_schema = "<database_name>";
```
- View procedures
```sh
show procedure status;
```
- Drop a procedure 
```sh
DROP PROCEDURE IF EXISTS procedureName;
```
- Desc procedure
```sh
show create procedure procedureName;
```