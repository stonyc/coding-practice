https://www.hackerrank.com/challenges/weather-observation-station-6/problem

```sql
SELECT DISTINCT CITY FROM STATION WHERE POSITION("A" IN CITY)=1 \
OR POSITION("E" IN CITY)=1 OR POSITION("I" IN CITY)=1 \
OR POSITION("O" IN CITY)=1 OR POSITION("U" IN CITY)=1;
```
