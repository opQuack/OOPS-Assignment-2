```sql

DECLARE
    SAL FLOAT;
    EXP INTEGER;
    BONUS FLOAT;
    TOTAL FLOAT;
BEGIN
    SAL := 12500;
    EXP := 12;
    BONUS := 0.1*SAL;
    if(EXP > 10)then
        BONUS := BONUS +  500;
    end if;
    TOTAL := SAL + BONUS;
    dbms_output.put_line('SALARY: ' || SAL);
    dbms_output.put_line('BONUS: ' || BONUS);
    dbms_output.put_line('TOTAL: ' || TOTAL);
END;
/

```
