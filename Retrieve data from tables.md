## Retrieve data from tables
### 1. Write a SQL statement to display all the information of all salesmen.
```SQL
SELECT *
FROM salesman;
```

### 2. Write a SQL statement to display a string "This is SQL Exercise, Practice and Solution".
```SQL
SELECT "This is SQL Exercise, Practice and Solution";
```

### 3. Write a query to display three numbers in three columns.
```SQL
SELECT 1, 2, 3;
```

### 4. Write a query to display the sum of two numbers 10 and 15 from RDMS sever.
```SQL
SELECT 5 + 10;
```

### 5. Write a query to display the result of an arithmetic expression.
```SQL
SELECT 5 + 10 * 2 - 15;
```

### 6. Write a SQL statement to display specific columns like name and commission for all the salesmen. 
```SQL
SELECT name, commission
FROM salesman;
```

### 7. Write a query to display the columns in a specific order like order date, salesman id, order number and purchase amount from for all the orders.
```SQL
SELECT ord_date, salesman_id, ord_no, purch_amt
FROM orders;
```

### 8. Write a query which will retrieve the value of salesman id of all salesmen, getting orders from the customers in orders table without any repeats.
```SQL
SELECT DISTINCT salesman_id
FROM orders;
```

### 9. Write a SQL statement to display names and city of salesman, who belongs to the city of Paris.
```SQL
SELECT name, city
FROM salesman
WHERE city = 'Paris';
```

### 10. Write a SQL statement to display all the information for those customers with a grade of 200.
```SQL
SELECT *
FROM customer
WHERE grade = 200;
```

### 11. Write a SQL query to display the order number followed by order date and the purchase amount for each order which will be delivered by the salesman who is holding the ID 5001.
```SQL
SELECT ord_no, ord_date, purch_amt
FROM orders
WHERE salesman_id = 5001;
```

### 12. Write a SQL query to display the Nobel prizes for 1970.
```SQL
SELECT *
FROM nobel_win
WHERE YEAR = 1970;
```

### 13. Write a SQL query to know the winner of the 1971 prize for Literature.
```SQL
SELECT *
FROM nobel_win
WHERE YEAR = 1971 AND SUBJECT = 'Literature';
```

### 14. Write a SQL query to display the year and subject that won 'Dennis Gabor' his prize.
```SQL
SELECT YEAR, SUBJECT
FROM nobel_win
WHERE WINNER = 'Dennis Gabor';
```

### 15. Write a SQL query to give the name of the 'Physics' winners since the year 1950.
```SQL
SELECT WINNER
FROM nobel_win
WHERE SUBJECT = 'Physics' AND YEAR >= 1950;
```