# TechTFQ_SQL_Interview_Query_26

PROBLEM STATEMENT:
Given table contains tokens taken by different customers in a tax office.
Write a SQL query to return the lowest token number which is unique to a customer (meaning token should be allocated to just a single customer).

```sql
drop table if exists tokens;
create table tokens

(
	token_num	int,
	customer	varchar(20)
);
insert into tokens values(1, 'Maryam');
insert into tokens values(2, 'Rocky');
insert into tokens values(3, 'John');
insert into tokens values(3, 'John');
insert into tokens values(2, 'Arya');
insert into tokens values(1, 'Pascal');
insert into tokens values(9, 'Kate');
insert into tokens values(9, 'Ibrahim');
insert into tokens values(8, 'Lilly');
insert into tokens values(8, 'Lilly');
insert into tokens values(5, 'Shane');

select * from tokens;
```

| token_num | customer |
|-----------|----------|
| 1	 | Maryam | 
| 2	| Rocky |
| 3	 | John |
| 3	| John |
| 2	 | Arya |
| 1	 | Pascal |
| 9	 | Kate |
| 9	 | Ibrahim |
| 8	 | Lilly |
| 8	 | Lilly |
| 5	 | Shane |
