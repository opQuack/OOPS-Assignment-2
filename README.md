```sql

BEGIN
    FOR item in (Select * from Employee)
    LOOP
        dbms_output.put_line(item.NAME || ' ' || item.JOB || ' ' || item.SALARY || ' ' || item.DEPT);
    END LOOP;
END;
/

```
