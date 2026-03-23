### Exercise 2:

## Q1 Find the movie with a row id of 6 ✓
```sql

SELECT * FROM movies
WHERE id = 6;
```
## Q2: Find the movies released in the years between 2000 and 2010
```sql
SELECT year
FROM movies
WHERE year BETWEEN 2000 AND 2010;
```

## Q3:Find the movies not released in the years between 2000 and 2010
```sql
SELECT year
FROM movies
WHERE year not BETWEEN 2000 AND 2010;
```
## Q4: Find the first 5 Pixar movies and their release year
```sql
SELECT title FROM movies
order by YEAR asc
limit 5;
```