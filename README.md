```sql

DECLARE
    empNo employee.ID%type;
    SALARY employee.SALARY%TYPE;
    maxSALARY employee.SALARY%TYPE;
    minSALARY employee.SALARY%TYPE;
    empName employee.NAME%TYPE;
BEGIN
    Select min(Salary), max(Salary) INTO minSALARY, maxSALARY 
    from employee;
    
    Select ID, Name INTO empNo, empName
    from employee
    where Salary = minSALARY;
    
    dbms_output.put_line('MINIMUM SALARY');
    dbms_output.put_line('ID: ' || empNo);
    dbms_output.put_line('Name: ' || empName);
    
    Select ID, Name INTO empNo, empName
    from employee
    where Salary = maxSALARY;
    
    dbms_output.put_line('MAXIMUM SALARY');
    dbms_output.put_line('ID: ' || empNo);
    dbms_output.put_line('Name: ' || empName);
END;
/
    
    

```
