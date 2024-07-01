#hackerrank #SQL #bronze_star #regex 

[Weather Observation Station 7 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-7/problem?isFullScreen=true)

Query the list of _CITY_ names ending with vowels (a, e, i, o, u) from **STATION**. Your result _cannot_ contain duplicates.
**Input Format**
The **STATION** table is described as follows:
![[Pasted image 20240604105234.png]]
where _LAT_N_ is the northern latitude and _LONG_W_ is the western longitude.

THE QUERY:
```sql

SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP"([AEIOU]$)";
```
- Again, just like before, same query except this time, we are checking for the ending character with `$` sign. For more info on #regex, checkout **[[Regular Expression Pattern]]**.

[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-6?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 6]].
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-8?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 8]].

For more info on regex, consider reading [[Regular Expression Pattern]].