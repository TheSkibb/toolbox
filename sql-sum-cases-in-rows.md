~~~sql
SELECT
  SUM(CASE WHEN your_column = 'yes' THEN 1 ELSE 0 END) AS yes,
  SUM(CASE WHEN your_column = 'no' THEN 1 ELSE 0 END) AS no
FROM your_table;
~~~
