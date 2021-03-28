```sql

DECLARE
    empNo INTEGER;
    SALARY employee.SALARY%TYPE;
    empName employee.NAME%TYPE;
BEGIN
    empNo := &empNo;
    Select Salary, Name INTO SALARY, empName 
    from employee
    where ID = empNo;
    dbms_output.put_line('ID: ' || empNo);
    dbms_output.put_line('Name: ' || empName);
    dbms_output.put_line('Salary: ' || empNo);
END;
/
    

```
