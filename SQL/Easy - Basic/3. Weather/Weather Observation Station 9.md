#hackerrank #SQL #bronze_star #regex 

[Weather Observation Station 9 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-9/problem?isFullScreen=true)

Query the list of _CITY_ names from **STATION** that _do not start_ with vowels. Your result cannot contain duplicates.
**Input Format**
The **STATION** table is described as follows:
![[Pasted image 20240604114452.png]]
where _LAT_N_ is the northern latitude and _LONG_W_ is the western longitude.
THE QUERY:
```sql

SELECT DISTINCT CITY FROM STATION WHERE CITY NOT REGEXP'(^[AEIOU])';
```
- All things similar to [[Weather Observation Station 6]], except, we're gonna be using another *simple keyword* `NOT`, which *basically puts the negative of the provided regex*.

[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-8?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 8]]
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-10?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 10]].

For more info on regex, consider reading [[Regular Expression Pattern]].