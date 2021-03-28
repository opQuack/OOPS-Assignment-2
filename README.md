```sql

DECLARE
    empno INTEGER;
    SALARY employee.salary%type;
BEGIN
    empno := 2;
    
    SELECT Salary INTO SALARY
    from Employee 
    where ID = empno;
    
    if(SALARY < 5000)then
        Update Employee
        SET Salary = Salary + 0.1*Salary
        where ID = empno;
    else
        DELETE from Employee
        where ID = empno;
    end if;
END;
/

Select * from Employee;
    

```
