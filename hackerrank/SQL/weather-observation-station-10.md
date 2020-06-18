https://www.hackerrank.com/challenges/weather-observation-station-10/problem

```sql
SELECT DISTINCT CITY FROM STATION WHERE \
RIGHT(CITY, 1) NOT IN ('A','E','I','O','U');
```
