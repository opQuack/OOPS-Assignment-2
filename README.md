```sql

DECLARE
    Y INTEGER;
BEGIN
    Y := 1996;
    
    if(mod(Y,4) = 0)then
        if(mod(Y,100) = 0 and mod(Y,400) != 0)then
            dbms_output.put_line(Y || ': NOT Leap Year');
        else
            dbms_output.put_line(Y || ': Leap Year');
        end if;
    end if;
END;
/

```
