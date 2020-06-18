https://www.hackerrank.com/challenges/what-type-of-triangle/problem

```sql
SELECT 
CASE
  WHEN A=B AND B=C THEN 'Equilateral'
  WHEN A+B<=C THEN 'Not A Triangle'
  WHEN A=B THEN 'Isosceles'
  ELSE 'Scalene'
END FROM TRIANGLES;
```
