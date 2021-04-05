```sql

CREATE TABLE employee(
    ID INT,
    NAME VARCHAR (20) NOT NULL,
    AGE INT NOT NULL,
    DEPT VARCHAR(25),
    ADDRESS CHAR (25),
    SALARY DECIMAL (18, 2),
    PRIMARY KEY (ID)
);

INSERT INTO employee VALUES (1, 'Anshuman', 32, 'Accounts', 'Kanpur', 2000.00 );
INSERT INTO employee VALUES (2, 'Priyanshu', 25, 'HR', 'Delhi', 1500.00 );
INSERT INTO employee VALUES (3, 'Satvik', 23, 'Engineering', 'Hyderabad', 2000.00 );
INSERT INTO employee VALUES (4, 'Pankaj', 25, 'Accounts', 'Rajasthan', 6500.00 );
INSERT INTO employee VALUES (5, 'Rohit', 27, 'HR', 'Vizag', 8500.00 );
INSERT INTO employee VALUES (6, 'Shikhar', 22, 'Engineering', 'Allahabad', 4500.00 );

```
