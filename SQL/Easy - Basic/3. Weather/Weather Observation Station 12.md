#hackerrank #SQL #bronze_star #regex 

[Weather Observation Station 12 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-12/problem?isFullScreen=true)

Query the list of _CITY_ names from **STATION** that _do not start_ with vowels and _do not end_ with vowels. Your result cannot contain duplicates.
**Input Format**
The **STATION** table is described as follows:
![[Pasted image 20240604170732.png]]
where _LAT_N_ is the northern latitude and _LONG_W_ is the western longitude.
THE QUERY:
```sql

SELECT DISTINCT CITY FROM STATION WHERE CITY NOT REGEXP'(^[AEIOU])' AND CITY NOT REGEXP'([AEIOU]$)';
```
- And like [[Weather Observation Station 11]], it's pretty much the same except for condition given in problem statement. Instead of `OR`, it states `AND`. **Pretty dumb hint if you ask me!**

[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-11?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 11]].
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-13?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 13]].

For more info on regex, consider reading [[Regular Expression Pattern]].