## Using Boolean and Relational operators
### 1. Write a query to display all customers with a grade above 100.   
```SQL
SELECT *
FROM customer
WHERE grade > 100;
```

### 2. Write a query statement to display all customers in New York who have a grade value above 100.
```SQL
SELECT *
FROM customer
WHERE grade > 100 AND city = 'New York';
```

### 3. Write a SQL statement to display all customers, who are either belongs to the city New York or had a grade above 100. 
```SQL
SELECT *
FROM customer
WHERE grade > 100 OR city = 'New York';
```

### 4. Write a SQL statement to display all the customers, who are either belongs to the city New York or not had a grade above 100.
```SQL
SELECT *
FROM customer
WHERE NOT grade > 100 OR city = 'New York';
```

### 5.Write a SQL query to display those customers who are neither belongs to the city New York nor grade value is more than 100.
```SQL
SELECT *
FROM customer
WHERE NOT (grade > 100 OR city = 'New York');
```

### 6. Write a SQL statement to display either those orders which are not issued on date 2012-09-10 and issued by the salesman whose ID is 505 and below or those orders which purchase amount is 1000.00 and below.  
```SQL
SELECT *
FROM orders
WHERE ord_date != '2012-09-10'
  AND salesman_id <= 505
  OR purch_amt <= 1000;

```