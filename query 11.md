### EXERCISE 11
### 1 Find the number of Artists in the studio (without a HAVING clause)
```SQL
SELECT COUNT(*) 
FROM employees
WHERE role = 'Artist';
```


### 2 Find the number of Employees of each role in the studio
```SQL
SELECT role,
       AVG(years_employed) AS avg_years
FROM employees
GROUP BY role;
```
### 3 Find the total number of years employed by all Engineers
```SQL
SELECT SUM(years_employed) 
FROM employees
WHERE role = 'Engineer';
```
