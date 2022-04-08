# mysql-stored-functions
mysqlsampledatabse.sql file is taken from mysqltutorial.org
Note : “Deterministic” Keyword : A deterministic function always returns the same result for the same input parameters whereas a non-deterministic function returns different results for the same input parameters.
If you don’t use DETERMINISTIC or NOT DETERMINISTIC, MySQL uses the NOT DETERMINISTIC option by default.
1. employee(empid,fname,lname,start_date)
   Write Mysql function “no_of_years” to find the number of years the employee has been in the company.
   Write SQL query to find employee details along with number of years he has been with the company.
2. customer(customerNumber,customerName,creditLimit)
    Write Mysql function “calculate_level” that returns the customer level based on credit.(Above 50000 customer level is “platinum”, between 50000 to 10000 customer level is “gold”, less than 10000 customer level is “silver”)
3. products (prod_id, prod_name, prod_cost, prod_price);

  Write Mysql function “calcProfit”  which calculates the profit by subtracting the cost from the price, and then returns the value to the calling expression.

4. Write Mysql function “WEIGHTED_AVERAGE” that assigns a weight of 1 to n1, 1 to n2, 2 to n3, 4 to n4 to calculate the weighted average.

5. studentdata(name, mark1, mark2, mark3, mark4)

   Write Mysql function “WEIGHTED_AVERAGE2” that assigns a weight of 1 to mark1, 1 to mark2, 2 to mark3, 4 to mark4 to calculate the weighted average given the student name.

6. studentdata(name, mark1, mark2, mark3, mark4)

Write Mysql function “WEIGHTED_AVERAGE3” to insert the student data into the table studentdata. Assign a weight of 1 to mark1, 1 to mark2, 2 to mark3, 4 to mark4. Marks and name are given as parameters to the function.

7. studentdata(name, mark1, mark2, mark3, mark4)

Write Mysql function “WEIGHTED_AVERAGE_UPDATE” to to update a student record given his name.

8. Write Mysql function “CalcIncome” to calculate Income. Income is calculated as m times starting value such that m*starting value < 3000. starting_value is parameter to the function.m should be as smaller as possible. 
8.product(pid,pname,normal_price)
  Write Mysql function “f_discount_price” to calculate the discount price of a product given it`s normal price. If normal price is greater than 500 then discounted price is 0.8 * normal_price, is normal price is greater than 100 then discounted price is 0.9*normal_price.
9.rentalMovies(movie_id,membership number,return_date)

Suppose we want to know which rented movies are past the return date. Create a stored function “sf_past_movie_return_date” that accepts the return date as the parameter and then compares it with the current date in MySQL server. If the current date is less than the return movie date, then we return “No” else we return “Yes”. 

10. emp(empid,name,salary)

      Write Mysql function “get_salary” to fetch an employee`s salary given his empid.

Difference between “stored procedure” and “stored function”.
 


