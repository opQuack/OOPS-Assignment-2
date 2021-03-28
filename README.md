```sql

DECLARE
    PRINCIPAL FLOAT;
    TI INTEGER;
    RATE FLOAT;
    SI FLOAT;
    TOTAL FLOAT;
BEGIN
    PRINCIPAL := 5600;
    TI := 12;
    if(TI > 10)then
        RATE := 0.08;
    else
        RATE := 0.06;
    end if;
    SI := PRINCIPAL*RATE*TI;
    TOTAL := PRINCIPAL + SI;
    dbms_output.put_line('P: ' || PRINCIPAL);
    dbms_output.put_line('T: ' || TI);
    dbms_output.put_line('R: ' || RATE*100 || '%');
    dbms_output.put_line('SI: ' || SI);
    dbms_output.put_line('TOTAL: ' || TOTAL);
END;
/

```
