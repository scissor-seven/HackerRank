#hackerrank #SQL #bronze_star #regex 

[Weather Observation Station 11 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-11/problem?isFullScreen=false)

Query the list of _CITY_ names from **STATION** that either do not start with vowels or do not end with vowels. Your result cannot contain duplicates.
**Input Format**
The **STATION** table is described as follows:
![[Pasted image 20240604153712.png]]
where _LAT_N_ is the northern latitude and _LONG_W_ is the western longitude.
THE QUERY:
```sql

SELECT DISTINCT CITY FROM STATION WHERE CITY NOT REGEXP'(^[AEIOU])' OR CITY NOT REGEXP'([AEIOU]$)';
```
- Unlike before, we cannot just join both character class with `.*` in middle cause that will put negative of `.*` as well, which we probably don't want.
- Therefore, we write 2 separate `regexp()` with an `OR` just as said in the problem statement.

[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-10?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 10]].
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-12?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 12]].

For more info on regex, consider reading [[Regular Expression Pattern]].