#hackerrank #SQL #bronze_star #regex 

[Weather Observation Station 8 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-8/problem?isFullScreen=true)

Query the list of _CITY_ names from **STATION** which have vowels (i.e., _a_, _e_, _i_, _o_, and _u_) as both their first _and_ last characters. Your result cannot contain duplicates.
**Input Format**
The **STATION** table is described as follows:
![[Pasted image 20240604113054.png]]
where _LAT_N_ is the northern latitude and _LONG_W_ is the western longitude.
THE QUERY:
```sql

SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP'(^[AEIOU].*[AEIOU]$)';
```
- Once again an encounter with a similar query except for the `.*` part, which means 2 things.
	- `.` mean any single character
	- `*` means zero or more times the number of character before this sign, meaning `'.'` (ignore the quotes!).

[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-7?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 7]].
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-9?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 9]].

For more info on regex, consider reading [[Regular Expression Pattern]].