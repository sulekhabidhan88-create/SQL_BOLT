### Exercise 5: 
## Q1: List all the Canadian cities and their populations
```sql
SELECT city, population
FROM north_american_cities
WHERE country = "Canada";
```
## Q2: Order all the cities in the United States by their latitude from north to south
```sql
SELECT city, latitude
FROM north_american_cities
WHERE country = "United States"
order by latitude DESC ;
```

## Q3:List all the cities west of Chicago, ordered from west to east
```sql
SELECT city, longitude
FROM north_american_cities
WHERE Longitude < (SELECT longitude FROM north_american_cities WHERE city = "Chicago")
order by longitude asc
```
## Q4:List the two largest cities in Mexico (by population)
```sql
SELECT city, population
FROM north_american_cities
WHERE country = 'Mexico'
order by population DESC
LIMIT 2;
```

## Q5:List the third and fourth largest cities (by population) in the United States and their population
```sql
SELECT city, population
FROM north_american_cities
WHERE country = 'United States'
order by population DESC
LIMIT 2 OFFSET 2;
```