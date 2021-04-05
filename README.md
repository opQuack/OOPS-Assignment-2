```sql

BEGIN
    FOR item in (Select * from Employee)
    LOOP
        if(item.SALARY < 1200) then
            UPDATE employee
            SET SALARY = SALARY + 0.8*SALARY
            WHERE ID = item.ID;
        elsif(item.SALARY < 2500) then
            UPDATE employee
            SET SALARY = SALARY + 0.12*SALARY
            WHERE ID = item.ID;
        elsif(item.SALARY < 4500) then
            UPDATE employee
            SET SALARY = SALARY + 0.25*SALARY
            WHERE ID = item.ID;
        else
            UPDATE employee
            SET SALARY = SALARY + 0.20*SALARY
            WHERE ID = item.ID;
        end if;
    END LOOP;
END;
/

SELECT * FROM employee;

```
