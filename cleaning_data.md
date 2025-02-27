What issues will you address by cleaning the data?





Queries:
Below, provide the SQL queries you used to clean your data.

For question 1 I needed to remove NULL transaction values, so here is an example cleaning step to do that:

```sql
SELECT
	*
FROM
	all_sessions
WHERE total_transaction_revenue IS NOT NULL
```
