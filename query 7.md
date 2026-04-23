# EXPERIMENT-7
## Find the list of all buildings that have employees
```sql
SELECT DISTINCT b.building_name
FROM buildings b
INNER JOIN employees e
ON b.building_name = e.building;
```

## Find the list of all buildings and their capacity
```sql 
SELECT building_name, capacity
FROM buildings;
```
## List all buildings and the distinct employee roles in each building (including empty buildings)
```sql
SELECT DISTINCT b.building_name, e.role
FROM buildings b
LEFT JOIN employees e
ON b.building_name = e.building;
```
