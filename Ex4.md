### Exercise 4:

## Q1:List all directors of Pixar movies (alphabetically), without duplicates
```sql
SELECT DISTINCT director FROM movies
ORDER BY director asc;
```
## Q2: List the last four Pixar movies released (ordered from most recent to least)
```sql
SELECT title, year FROM movies
ORDER BY year DESC
LIMIT 4;
```
## Q3: List the first five Pixar movies sorted alphabetically
```sql
SELECT title FROM movies
ORDER BY title asc
LIMIT 5;
```
## Q4: List the next five Pixar movies sorted alphabetically
```sql
SELECT title FROM movies
ORDER BY title asc
LIMIT 5 OFFSET 5;
```