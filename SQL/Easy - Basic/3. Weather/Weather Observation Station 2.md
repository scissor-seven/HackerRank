#hackerrank #SQL #bronze_star 

[Weather Observation Station 2 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-2/problem?isFullScreen=true)

Query the following two values from the **STATION** table:

1. The sum of all values in _LAT_N_ rounded to a scale of `2` decimal places.
2. The sum of all values in _LONG_W_ rounded to a scale of `2` decimal places.

**Input Format**

The **STATION** table is described as follows:
![[Pasted image 20240603122343.png]]
where _LAT_N_ is the northern latitude and _LONG_W_ is the western longitude.

**Output Format**
Your results must be in the form:

```
lat lon
```

where ***lat*** is the sum of all values in _LAT_N_ and ***lon*** is the sum of all values in _LONG_W_. Both results must be rounded to a scale of `2` decimal places.

THE QUERY:
```SQL

SELECT ROUND(SUM(LAT_N), 2), ROUND(SUM(LONG_W), 2) FROM STATION;
```
EXPLANATION:
- Only 2 things need explanation here, `ROUND()` & `SUM()` functions.
- `ROUND()` takes 2 arguments, *first is the entity to round-off*, and *second is to which decimal place to round-off*.
- `SUM()` function simply **takes a column_name as an argument and sum up its data!** *Mostly it's used when data is numerical*, but also rarely in other cases as well!

[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-1?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 1]]
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-3?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 3]].