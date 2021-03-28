```sql

DECLARE
    Department employee.dept%type;
BEGIN
    Department := 'Accounts';
    
    DELETE from Employee
    where Dept = Department;
END;
/

Select * from Employee;

```
