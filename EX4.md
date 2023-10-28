# Ex. No: 4 Creating Procedures using PL/SQL

### AIM: 
To create a procedure using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

### Program:
```
Reg no. 212221230107
name: M.Sowmya
```
```
create database employee;
use employee;
CREATE TABLE employee (emp_id NUMERIC,emp_name VARCHAR(10),dept VARCHAR(10),salary NUMERIC);
DELIMITER //

CREATE PROCEDURE insert_employee()
BEGIN
    INSERT INTO employee (emp_id,emp_name,dept,salary)
    VALUES (1,'Sowmya','AI&DS',60000);
    
    INSERT INTO employee (emp_id,emp_name,dept,salary)
    VALUES (2,'Jhansi','CSE',50000);
    
    INSERT INTO employee (emp_id,emp_name,dept,salary)
    VALUES (3,'Ajitha','ECE',55000);
    
    commit;
    
end;
//
call insert_emp();
select *from employee;

```
### Output:
![Screenshot 2023-10-05 154005](https://github.com/MSowmya28/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/94154791/c284fdb7-f4fb-4fb0-b9b6-f03c06781924)


### Result:
The program has successfully executed.
