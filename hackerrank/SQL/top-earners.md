https://www.hackerrank.com/challenges/earnings-of-employees/problem

```sql
SELECT (months * salary) AS earnings, COUNT(*) \
FROM Employee GROUP BY 1 ORDER BY earnings DESC LIMIT 1;
```
