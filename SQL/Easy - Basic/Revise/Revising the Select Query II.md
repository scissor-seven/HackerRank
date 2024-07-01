#hackerrank #SQL #silver_star-3 #revise 
[Revising the Select Query II | HackerRank](https://www.hackerrank.com/challenges/revising-the-select-query-2/problem?isFullScreen=true)

Query the **NAME** field for all American cities in the **CITY** table with populations larger than `120000`. The _CountryCode_ for America is `USA`.
The **CITY** table is described as follows:
![[Pasted image 20240602210056.png]]
The query:
```sql

SELECT NAME FROM CITY WHERE POPULATION>120000 AND COUNTRYCODE='USA';
```

`NOTE: Remember to use single-quotes('') whenever passing on string as an input, like used in pushing 'USA' in` **CountryCode** `parameter`.
