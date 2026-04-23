###  EXPERIMENT-8
### 1 Find the name and role of all employees who have not been assigned to a building
```SQL
SELECT name, role
FROM employees
WHERE building IS NULL OR building = '';
```
### 2 Find the names of the buildings that hold no employees
```SQL
SELECT building_name
FROM buildings
LEFT JOIN employees
ON buildings.building_name = employees.building
WHERE employees.building IS NULL;
```
