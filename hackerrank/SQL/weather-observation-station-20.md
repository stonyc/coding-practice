https://www.hackerrank.com/challenges/weather-observation-station-20

```sql
SELECT ROUND(LAT_N, 4) FROM STATION s 
WHERE (
    SELECT COUNT(LAT_N) FROM STATION WHERE LAT_N < s.LAT_N
) = (
    SELECT COUNT(LAT_N) FROM STATION WHERE LAT_N > s.LAT_N
);
```
