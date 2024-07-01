#hackerrank #SQL #bronze_star #regex 

[Weather Observation Station 10 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-10/problem?isFullScreen=true)

Query the list of _CITY_ names from **STATION** that _do not end_ with vowels. Your result cannot contain duplicates.
**Input Format**
The **STATION** table is described as follows:
![[Pasted image 20240604115155.png]]
where _LAT_N_ is the northern latitude and _LONG_W_ is the western longitude.
THE QUERY:
```sql

SELECT DISTINCT CITY FROM STATION WHERE CITY NOT REGEXP'([AEIOU]$)';
```
- And another one, same as before in [[Weather Observation Station 7]], except here, we'll be querying for the opposite, by using the `NOT` keyword!

[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-9?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 9]].
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-11?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 11]].

For more info on regex, consider reading [[Regular Expression Pattern]].