#hackerrank #SQL #bronze_star #regex 

[Weather Observation Station 6 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-6/problem?isFullScreen=true)

Query the list of _CITY_ names starting with vowels (i.e., `a`, `e`, `i`, `o`, or `u`) from **STATION**. Your result _cannot_ contain duplicates.
**Input Format**
The **STATION** table is described as follows:
![[Pasted image 20240604101111.png]]
where _LAT_N_ is the northern latitude and _LONG_W_ is the western longitude.

THE QUERY:
```sql

SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP"(^[AEIOU])";
```
- Alrighty, here comes the fun! Introduction with `REGEXP()` a.k.a **[[Regular Expression Pattern]]**.
- The `^` symbol matches for the beginning of the line being searched with the help of pattern.
- Except for the last part of this, rest is pretty much standard based on the problem statement. As for the `regexp()` function, make use of regular expression patterns for the ease of our search. **Think of it as an advanced level of searching/sorting!**

> **A regular expression pattern, often called a regex, is like a special code used to find and match specific text within a larger piece of text. Think of it as a search tool that can look for patterns rather than exact words.** ~ChatGPT 4o

[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-5?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 5]]
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-7?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 7]].

For more info on regex, consider reading [[Regular Expression Pattern]].