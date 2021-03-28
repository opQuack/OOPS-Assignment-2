```sql

DECLARE
    COUNTER INTEGER;
    SAL employee.Salary%type;
    EmpName employee.Name%type;
BEGIN
    SAL := &SAL;
    Select count(*) INTO COUNTER
    from Employee
    where Salary = SAL;
    
    if(COUNTER > 3)then
        RAISE TOO_MANY_ROWS;
    end if;
    
    Select Name INTO EmpName
    from Employee
    where Salary = SAL;
    
    dbms_output.put_line('Name: ' || EmpName);
    
EXCEPTION
    WHEN TOO_MANY_ROWS then
        dbms_output.put_line('TOO MANY ROWS');
    WHEN NO_DATA_FOUND then
        dbms_output.put_line('NO DATA FOUND');
END;
/

```
