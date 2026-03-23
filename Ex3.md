### Exercise 3:

## Q1:Find all the Toy Story movies
```sql
SELECT * FROM movies
WHERE title LIKE "toy Story%"
```
## Q2: Find all the movies directed by John Lasseter
```sql
SELECT * FROM movies
WHERE title LIKE "toy Story%"
```
## Q3: Find all the movies (and director) not directed by John Lasseter
```sql
SELECT * FROM movies
WHERE director != "John Lasseter"
```
## Q4: Find all the WALL-* movies
```sql
SELECT * FROM movies
WHERE title LIKE "WALL-%"
```