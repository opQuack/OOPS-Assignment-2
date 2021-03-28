```sql

DECLARE
    SAL FLOAT;
    HRA FLOAT;
    DA FLOAT;
    TOTAL FLOAT;
BEGIN
    SAL := 12500;
    if(SAL > 15000)then
        HRA := 0.12*SAL;
        DA := 0.08*SAL;
    elsif(SAL > 12000)then
        HRA := 0.10*SAL;
        DA := 0.06*SAL;
    elsif(SAL > 9000)then
        HRA := 0.07*SAL;
        DA := 0.04*SAL;
    else
        HRA := 0.05*SAL;
        DA := 500;
    end if;
    TOTAL := SAL + HRA + DA;
    dbms_output.put_line('SALARY: ' || SAL);
    dbms_output.put_line('HRA: ' || HRA);
    dbms_output.put_line('DA: ' || DA);
    dbms_output.put_line('TOTAL: ' || TOTAL);
END;
/

```
