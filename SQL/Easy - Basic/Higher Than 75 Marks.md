#hackerrank #SQL #silver_star-3 
[Higher Than 75 Marks | HackerRank](https://www.hackerrank.com/challenges/more-than-75-marks/problem?isFullScreen=true)

Query the _Name_ of any student in **STUDENTS** who scored higher than  _Marks_. Order your output by the _last three characters_ of each name. If two or more students both have names ending in the same last three characters (i.e.: Bobby, Robby, etc.), secondary sort them by ascending _ID_.

**Input Format**
The **STUDENTS** table is described as follows:
![[Pasted image 20240613125600.png]]
THE QUERY :
```sql

SELECT NAME FROM STUDENTS
WHERE MARKS > 75
ORDER BY SUBSTR(NAME, -3) , ID;
```

- The only unique thing here is, `order by` clause by default uses `asc` order. Therefore, without even using the keyword `ASC`, it's getting sorted in ascending.
- The `SUBSTR()` function in SQL is used to extract a substring from a given string.

Following is it's syntax:

**SUBSTRING(string, start, length)**
- `string`: The original string from which the substring will be extracted.
- `start`: The starting position for the extraction.
    - **A positive number starts from the beginning of the string (1-based index).**
    - **A negative number starts from the end of the string**.
- `length` (optional): The number of characters to extract. If omitted, the function extracts until the end of the string.