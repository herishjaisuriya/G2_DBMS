# EXP NO 1: DATA DEFINITION LANGUGE COMMANDS IN RDBMS

## AIM:
To create a student database and execute DDL queries using SQL.


## DDL (Data Definition Language)
<div align="justify">
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.
</div>
 
## List of DDL commands: 
<div align="justify">
CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
DROP: This command is used to delete objects from the database.
ALTER: This is used to alter the structure of the database.
TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
RENAME: This is used to rename an object existing in the database.
</div>

## Query:
### 1) Create a table student with the following fieds rollno,name,age,address,phoneno.

### SQL QUERY: 
```sql
CREATE TABLE student(roll_no NUMBER(5), name VARCHAR(20), age NUMBER(2), address VARCHAR(50), phone_no NUMBER(10));
```


### OUTPUT:
![image](https://github.com/dineshgl/G2_DBMS/assets/129932017/8b6457b6-ad87-4d24-8935-094e7c635464)


### 2) Change the above student table by adding another attribute department

### SQL QUERY: 
```sql
ALTER TABLE student ADD department VARCHAR(10);
```

### OUTPUT:
![image](https://github.com/dineshgl/G2_DBMS/assets/129932017/e6d4208b-6dc6-4836-808a-5216126f26a8)



### 3) Drop the student table
 
### SQL QUERY: 
```sql
DROP TABLE student;
```


### OUTPUT:
![image](https://github.com/dineshgl/G2_DBMS/assets/129932017/5ce09cee-04c1-48e7-ac79-faeeb58a3aed)


### 4) Delete the student table using truncate keyword

### SQL QUERY: 
```sql
TRUNCATE TABLE student;
```


### OUTPUT:
![image](https://github.com/dineshgl/G2_DBMS/assets/129932017/effc9433-ac76-46e2-90a8-1d04f4039a65)




### 5) Rename the student table to mystudent

### SQL QUERY: 
```sql
ALTER TABLE student RENAME TO my_student;
```


### OUTPUT:
![image](https://github.com/dineshgl/G2_DBMS/assets/129932017/b73f2fa0-87c7-4233-add0-45b183db38b4)

