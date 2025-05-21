What issues will you address by cleaning the data?





Queries:
Below, provide the SQL queries you used to clean your data.

## Cleaning Example 1

For question 1 I needed to remove NULL transaction values, so here is an example cleaning step to do that:

```sql
SELECT
	*
FROM
	all_sessions
WHERE total_transaction_revenue IS NOT NULL
```

| x | y | z |
|--|--|---|
| 1 | 2 | 3|
|4   | 5|    6|

I also needed to remove unknown cities from the data...

```sql
SELECT
	*
FROM
	all_sessions
WHERE city != 'not available in demo dataset'
```
