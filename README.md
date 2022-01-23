# SQL-Assignment-6
Q-1. Write an SQL query to print details of the Workers who have joined in Feb’2014.

Ans select * from worker
Where year(joining_date )=2014 and month(join_date)=2

Q-2. Write an SQL query to fetch duplicate records having matching data in some fields of
a table.

Ans select name, count(‘email’)
       From worker
       Group by name
      Having count(‘email)>1

Q-3. How to remove duplicate rows from Employees table.

Ans:  Select name, count (*)
      From worker
      Group by name
      Having count(*)>1

