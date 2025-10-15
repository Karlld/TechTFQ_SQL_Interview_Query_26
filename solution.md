```sql
WITH distinct_token AS (SELECT token_num,
                               COUNT(DISTINCT(customer)) AS dist_cust
                           FROM tokens
                           GROUP BY token_num
					   )
					   
	SELECT token_num 
	    FROM distinct_token
		WHERE dist_cust = 1 
		ORDER BY token_num ASC
		LIMIT 1;
```

| token_num |
|-----------|
| 3 |
