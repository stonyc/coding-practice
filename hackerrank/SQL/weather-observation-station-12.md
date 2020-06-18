https://www.hackerrank.com/challenges/weather-observation-station-12/problem

```sql
SELECT DISTINCT CITY FROM STATION WHERE \
LEFT(CITY, 1) NOT IN ('A','E','I','O','U') \
AND RIGHT(CITY, 1) NOT IN ('A','E','I','O','U');
```
