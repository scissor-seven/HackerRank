#hackerrank #SQL #silver_star-4 #medium #basic

[The PADS | HackerRank](https://www.hackerrank.com/challenges/the-pads/problem?isFullScreen=true)

I'll not be putting up the questions from here on out, so I'd suggest you read it in the problem itself very carefully.
As far as the queries are concerned, now that we have graduated from easy to medium, the change in level of queries is quite drastic comparatively.
So.... here we go!
As the P.S(Problem Statement) suggests, we have to use 2 different queries in order to achieve our goal.

*Here's query 1*:
- Apart from `select` itself, I assume rest is pretty clear, the `order by`.
- The `concat` function is what needs little explanation.
> This function combines several pieces of information into a `single string`
- The field names (`NAME, OCCUPATION`) from where the record is required are mentioned as is, with *characters*, which are to be *presented in their true forms*, such as *brackets or specific strings*, are put under `' '` **single quotes**.
>For example the `'('` and such.
- The `left` function in first query is used to specify any character from left in a record from field, specified by comma separated integer.
> LEFT(OCCUPATION, 1) - First character of record from Occupation field!
- That'll be it for the first query.
```sql

SELECT CONCAT(NAME, '(', LEFT(OCCUPATION, 1), ')') 
FROM OCCUPATIONS 
ORDER BY NAME;
```

*Here's query 2*:
- Just as previous query, I assume the `group by` and `order by` functions are pretty much understood. But yes, the *sequence of mentioning* in `order by` *does matter*, because of what is mentioned in ***explanation*** at the end of P.S.
- As for the `concat` function in `select`, here's how it works:
	- As explained in previous query, about what `concat` does, how it can be used, regarding strings and using ***field records***.
	- The `count(*)` function is counting number of all the occupations individually.
	- And for `lower` function, it's used to *output field record in lowercase*.

```sql

SELECT CONCAT('There are a total of ', COUNT(*), ' ', LOWER(Occupation), 's.') 
FROM OCCUPATIONS 
GROUP BY Occupation 
ORDER BY COUNT(*), Occupation;
```