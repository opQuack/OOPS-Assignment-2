```sql

CREATE TABLE employee(
    ID INT,
    NAME VARCHAR (20) NOT NULL,
    AGE INT NOT NULL,
    JOB VARCHAR(25),
    DEPT VARCHAR(25),
    ADDRESS CHAR (25),
    SALARY DECIMAL (18, 2),
    PRIMARY KEY (ID)
);

INSERT INTO employee VALUES (1, 'Anshuman', 32, 'MANAGER', 'Accounts', 'Kanpur', 2000.00 );
INSERT INTO employee VALUES (2, 'Priyanshu', 25, 'ASSISTANT', 'HR', 'Delhi', 1500.00 );
INSERT INTO employee VALUES (3, 'Satvik', 23, 'JUNIOR', 'Engineering', 'Hyderabad', 2000.00 );
INSERT INTO employee VALUES (4, 'Pankaj', 25, 'GENERAL MANAGER', 'Accounts', 'Rajasthan', 6500.00 );
INSERT INTO employee VALUES (5, 'Rohit', 27, 'SUBORDINATE', 'HR', 'Vizag', 8500.00 );
INSERT INTO employee VALUES (6, 'Shikhar', 22, 'HOD', 'Engineering', 'Allahabad', 4500.00 );

```
