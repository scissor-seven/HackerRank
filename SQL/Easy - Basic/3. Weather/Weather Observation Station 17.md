#hackerrank #SQL #bronze_star 

[Weather Observation Station 17 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-17/problem?isFullScreen=true)

Query the _Western Longitude_ (_LONG_W_)where the smallest _Northern Latitude_ (_LAT_N_) in **STATION** is greater than `38.7780`. Round your answer to `4` decimal places.
**Input Format**
The **STATION** table is described as follows:
![[Pasted image 20240607124622.png]]
where _LAT_N_ is the northern latitude and _LONG_W_ is the western longitude.
THE QUERY:
```sql

SELECT ROUND(LONG_W, 4) FROM STATION WHERE LAT_N=(SELECT MIN(LAT_N) FROM STATION WHERE LAT_N>38.7780);
```
- Nothing much to explain here as well, because we attempted something similar in [[Weather Observation Station 15]]. Refer to that and you'll probably understand what's going on here!
- If you still don't understand, relax, meditate for a bit, calm and clear your mind, then read that again. **Now you'll definitely understand!**

[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-16/problem?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 16]].

------------------------------------------------------------------
The `easy difficulty` `Weather Observation Station` series on `basic level` ends here!
It is continued on `Medium Difficulty` here -> [[Weather Observation Station 18]].

------------------------------------------------------------------