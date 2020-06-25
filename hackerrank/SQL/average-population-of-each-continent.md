https://www.hackerrank.com/challenges/average-population-of-each-continent/problem

```sql
SELECT c.CONTINENT, FLOOR(AVG(ct.POPULATION)) \
FROM CITY ct INNER JOIN COUNTRY c \
ON ct.COUNTRYCODE=c.CODE GROUP BY c.CONTINENT;
```
