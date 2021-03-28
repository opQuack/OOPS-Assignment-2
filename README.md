```sql

DECLARE
    num1 INTEGER;
    num2 INTEGER;
    sum_val INTEGER;
    average FLOAT;
BEGIN
    num1 := 2;
    num2 := 3;
    sum_val := num1 + num2;
    average := sum_val/2;
    dbms_output.put_line('Num 1: ' || num1);
    dbms_output.put_line('Num 2: ' || num2);
    dbms_output.put_line('Total: ' || sum_val);
    dbms_output.put_line('Average: ' || average);
END;
/
```
