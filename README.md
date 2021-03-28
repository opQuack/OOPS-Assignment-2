```sql

DECLARE
    NUM1 INTEGER;
    NUM2 INTEGER;
    INVALID_GREATNESS EXCEPTION;
BEGIN
    NUM1 := 20;
    NUM2 := 5;
    if(NUM2 > NUM1)then
        RAISE INVALID_GREATNESS;
    end if;
    dbms_output.put_line('ANS: ' || NUM1/NUM2);
EXCEPTION
    WHEN INVALID_GREATNESS then
        dbms_output.put_line('NUM2 > NUM1');
    WHEN ZERO_DIVIDE then
        dbms_output.put_line('Divide by Zero');
END;
/

```
