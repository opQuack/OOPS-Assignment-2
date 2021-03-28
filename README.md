```sql

DECLARE
    empID employee.id%TYPE;
    empAddress employee.address%TYPE;
    empName employee.name%TYPE;
    empAge employee.age%TYPE;
    empSal employee.salary%TYPE;
    empDept employee.Dept%TYPE;
BEGIN 
    empID := 8;
    empName := 'Jeff';
    empAge := 28;
    empAddress := 'Mumbai';
    empSal := 2700;
    empDept := 'HR';
    INSERT INTO employee VALUES(empID,empName,empAge,empAddress,empSal, empDept);
END;
/

Select * from Employee;

```
