# PostgreSQL
Going to cover all PostgreSQL topic in depth
<h3>CONCAT_WS() Function</h3>

```
Select concat_ws (':' , emp_id, fname, lname, dept) from employees
where emp_id = 1;

o/p -[ 1:Raj:Sharma:IT ]

```
<h3>CONCAT_WS() Inside CONCAT_WS() Function</h3>
```

select concat_ws(':', emp_id, CONCAT_WS(' ', fname, lname), dept) from employees
where emp_id = 1;  

o/p - [ 1:Raj Sharma:IT ]
 
```

