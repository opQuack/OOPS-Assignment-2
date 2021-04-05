```sql

DECLARE
    DEPARTMENT VARCHAR(25);
BEGIN
    DEPARTMENT := 'Accounts';
    FOR item in (Select * from Employee where dept = DEPARTMENT)
    LOOP
        dbms_output.put_line(item.name || ' ' || item.job || ' ' || item.salary);
    END LOOP;
END;
/

```
