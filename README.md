# Hello all, I am sharing how to use WHERE function in SQL  

### Where statement allows us to apply specific conditions on columns for the rows to be returned.  
### In Simple terms it is used to aplly any filter conditions.  

* Syntax =  
```
SELECT column_1, column_2 FROM table_name  
WHERE condition ;
```
### WHERE clause appears immediately after the FROM clause of the SELECT statement.  

+ Comparison operator  

![Comparison Operator Table](./Comparison%20operator.jpg)  

+ Logical Operator = AND, OR, NOT  

## Examples  
Let's assume there is table namd T1 where name of person and their color choice is given.  

![Name](Name%20Table.jpg)  

1. Select the name 'David' from the table.
```
SELECT Name, Choice from T1
Where name = 'David';
```

2. Select the person named David whose choice is red.
```
SELECT Name, Choice FROM T1
WHERE name = 'David' AND Choice = 'Red';
```  

### In same manner we can apply *comparison operators* in any table we want.  

## Examples  
1. This code will give the list of all the films whose rental rate is more than 4$. 
```
SELECT film_title FROM table_name
WWHEREhere rental_rate > 4;
```  

2. This code will give the list of all the films whose rental rate is more than 4$ and replacement cost is more than or equal to 19.99$ and rating is 'R'. 
```
SELECT film_title from table_name
WHERE rental_rate > 4 AND replacement_cost >= 19.99
AND rating = 'R';
```  

3. Suppose we have a table T2 which contains email, first name and last name of customers. A customer forgot their wallet at our store and we need to track down their email to inform them. Find the email of the customer with name 'Nancy Thomas'.  
```
SELECT email, first_name, last_name FROM T2
WHERE first_name = 'Nancy' AND last_name = 'Thomas';
```  

4. Suppose we have a table T3 which contains film title and discription of the movie. A customer wants to know what the movie "Hello" is about. Could you give the decsriotion of the mentioned movie.
```
SELECT title, description FROM T3
WHERE title = 'Hello':
```  
## That's it for the WHERE functions, see you in the next chapter !!

            


