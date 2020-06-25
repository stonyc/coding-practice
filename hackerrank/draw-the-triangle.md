https://www.hackerrank.com/challenges/draw-the-triangle-1

**NOTE:** HackerRank doesn't all stored procedures using MySQL, so `WHILE` loop isn't possible without some trickery.**

```sql
SELECT
REPEAT('* ', COUNT.N)
FROM
(
    SELECT 20 AS N
    UNION ALL SELECT 19
    UNION ALL SELECT 18
    UNION ALL SELECT 17
    UNION ALL SELECT 16
    UNION ALL SELECT 15
    UNION ALL SELECT 14
    UNION ALL SELECT 13
    UNION ALL SELECT 12
    UNION ALL SELECT 11
    UNION ALL SELECT 10
    UNION ALL SELECT 9
    UNION ALL SELECT 8
    UNION ALL SELECT 7
    UNION ALL SELECT 6
    UNION ALL SELECT 5
    UNION ALL SELECT 4
    UNION ALL SELECT 3
    UNION ALL SELECT 2
    UNION ALL SELECT 1
) AS COUNT;
```
