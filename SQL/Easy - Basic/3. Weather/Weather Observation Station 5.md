#hackerrank #SQL #bronze_star 

[Weather Observation Station 5 | HackerRank](https://www.hackerrank.com/challenges/weather-observation-station-5/problem?isFullScreen=true)

Query the two cities in **STATION** with the shortest and longest _CITY_ names, as well as their respective lengths (i.e.: number of characters in the name). If there is more than one smallest or largest city, choose the one that comes first when ordered alphabetically.  
The **STATION** table is described as follows:
![[Pasted image 20240603131913.png]]
where **LAT_N** is the northern latitude and **LONG_W** is the western longitude.

**Sample Input**

For example, **CITY** has four entries: **DEF, ABC, PQRS** and **WXY**.

**Sample Output**

```
ABC 3
PQRS 4
```

**Explanation**

When ordered alphabetically, the **CITY** names are listed as **ABC, DEF, PQRS,** and **WXY**, with lengths `3, 3, 4` and 3. The longest name is **PQRS**, but there are 3 options for shortest named city. Choose **ABC**, because it comes first alphabetically.
**Note**  
You can write two separate queries to get the desired output. It need not be a single query.

**A great problem to solve covering multiple concepts...!**
THE QUERY:
```SQL

SELECT CITY, LENGTH(CITY) FROM STATION ORDER BY LENGTH(CITY) ASC, CITY ASC LIMIT 1;

SELECT CITY,LENGTH(CITY) FROM STATION ORDER BY LENGTH(CITY) DESC, CITY ASC LIMIT 1;
```
This one has a lot to explain:
- Query No. 1
```SQL

SELECT CITY, LENGTH(CITY) FROM STATION ORDER BY LENGTH(CITY) ASC, CITY ASC LIMIT 1;
```

- The `select` part states 2 arguments to select, `CITY` & `LENGTH(CITY)`. Length function will consider the character length in a city's name.
- `ORDER BY` can be said as a filter for sorting, in our case its the contents from select part.
- `LENGTH(CITY) ASC` means *sort in an ascending manner of length of characters*. From smallest city name to biggest city name.
- `CITY ASC LIMIT 1` says to choose the name in *ascending order of city names*, like if there are 3 cities, `C, A & B` then the ascending order will be `A, B & C`, with *selection limit of 1*.

- Query No. 2
```sql

SELECT CITY,LENGTH(CITY) FROM STATION ORDER BY LENGTH(CITY) DESC, CITY ASC LIMIT 1;
```
- This is similar to every aspect with the previous query **except** this time, we are ordering to select `length(city) desc`, meaning choose **the only longest city name**, with `CITY ASC LIMIT 1`, in ascending order of their name!

Thus solving this problem with the above 2 queries!
[Previous Challenge](https://www.hackerrank.com/challenges/weather-observation-station-4?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 4]].
[Next Challenge](https://www.hackerrank.com/challenges/weather-observation-station-6?isFullScreen=true) <- is here, note is here -> [[Weather Observation Station 6]].