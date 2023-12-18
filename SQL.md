SQL Questions

W3School Questions:

Q1) Select all the different values from the Country column in the Customers table.
Ans: Select Distinct Country from Customers;

Q2) Select all records where the City column has the value "Berlin".
Ans: Select * from customers where City ="Berlin" ;

Q3) select all records where City is NOT "Berlin".
Ans: Select * from customers where not city = "Berlin"

Q4) Select all records where the CustomerID column has the value 32.
Ans: Select * from customers where customerid = 32;

Q5) Select all records where the City column has the value 'Berlin' and the PostalCode column has the value '12209'.
Ans: Select * from customers where city = "Berlin" and Postalcode = "12209";

Q6)Select all records where the City column has the value 'Berlin' or 'London'.
Ans: Select * from Customers where city ="Berlin" or city ="London"

Q7) Select all records where the value of the City column starts with the letter "a".
Ans: Select * from customers where city like 'a%' ;

Q8) Select all records where the value of the City column ends with the letter "a".
Ans: Select * from customers where city like '%a' ;

Q9) Select all records where the value of the City column contains the letter "a"
Ans: Select * from customers where city like '%a%' ;

Q10) Select all records where the value of the City column starts with letter "a" and ends with the letter "b"
Ans: Select * from customers where city like 'a%b';

Q11) Select all records where the value of the City column does NOT start with the letter "a"
Ans: Select * from customers where city not like 'a%' ;

Q12) select all the records where the value of the Price column is between 10 and 20.
Ans: Select * from Products where price between 10 and 20;

Q13)select all the records where the value of the Price column is NOT between 10 and 20.
Ans: Select * from products where price not between 10 and 20;

Q14)select all the records where the value of the ProductName column is alphabetically between 'Geitost' and 'Pavlova'.
Ans: Select * from products where ProductName  between 'Geitost' and 'Pavlova';

Q15)select all the records where Country is either "Norway" or "France".
Ans: Select * from Customers where country in ("Norway","France") ;

Q16) select all the records where Country is NOT "Norway" and NOT "France".
Ans: Select * from customers where country not in ('Norway','France');

Q17) Select all records from the Customers where the PostalCode column is NOT empty.
Ans: Select * from Customers where Postalcode is not null;

Q18) Select all records from the Customers where the PostalCode column is empty.
Ans: Select * from Customers where Postalcode is  null;



HackerRank Questions:

Q1) Query all columns for all American cities in the CITY table with populations larger than 100000. The CountryCode for America is USA.

Ans: Select * from CITY
WHERE Population > 100000 and CountryCode = 'USA'  ;

Q2) Query the NAME field for all American cities in the CITY table with populations larger than 120000. The CountryCode for America is USA.

Ans: Query the NAME field for all American cities in the CITY table with populations larger than 120000. The CountryCode for America is USA.

Q3) Query all columns (attributes) for every row in the CITY table.

Ans: Select * from City;

Q4) Query all columns for a city in CITY with the ID 1661.
Ans: Select * from City where ID = 1661;

Q5) Query all attributes of every Japanese city in the CITY table. The COUNTRYCODE for Japan is JPN.
Ans: Select * from City where CountryCode = 'JPN';

Q6)Query the names of all the Japanese cities in the CITY table. The COUNTRYCODE for Japan is JPN.
Ans: Select NAME from City where CountryCode = 'JPN';

Q7) Query a list of CITY and STATE from the STATION table.
Ans: Select City,State from Station;

Q8)Query a list of CITY names from STATION for cities that have an even ID number. Print the results in any order, but exclude duplicates from the answer.
Ans: Select DISTINCT CITY FROM STATION 
WHERE MOD(ID,2) =0 ;

Q9) Find the difference between the total number of CITY entries in the table and the number of distinct CITY entries in the table.
Ans: SELECT COUNT(*) - COUNT(DISTINCT CITY)
FROM STATION;




W3Schools Questions Continued......

1) Select all records from the Customers table, sort the result alphabetically by the column City.

Ans: Select * from Customers ORDER BY City;

2) Select all records from the Customers table, sort the result reversed alphabetically by the column City.

Ans: Select * from Customers ORDER BY City DESC;

3)Select all records from the Customers table, sort the result alphabetically, first by the column Country, then, by the column City.

Ans: Select * from Customers ORDER BY Country,City;

4) Select all customers from Spain that starts with the letter 'G':

Ans: Select * from Customers where Country = "Spain" and Customername LIKE "G%" ;

5) selects all fields from Customers where Country is "Germany" AND City is "Berlin" AND PostalCode is higher than 12000

Ans: Select * from Customers
Where Country = "Germany"
AND City = "Berlin"
AND PostalCode >= 12000;

6) Select all Spanish customers that starts with either "G" or "R":

Ans: Select * from Customers where Country = "Spain"
AND Customername LIKE "G%" OR Customername LIKE "R%";

7) Select all customers that either are from Spain and starts with either "G", or starts with the letter "R"

Ans: Select * from Customers where Country = "Spain" and Customername LIKE "G%" 
OR Customername LIKE "R%";

8) Select all records where the City column has the value 'Berlin' and the PostalCode column has the value '12209'.

Ans: Select * from Customers where City= "Berlin" and PostalCode = 12209;

9) Select all records where the City column has the value 'Berlin' or 'London'

Ans: Select * from Customers where City = "Berlin" or City = 'London';


HackerRank Questions Continueddd.....

1) Query the sum of the populations for all Japanese cities in CITY. The COUNTRYCODE for Japan is JPN

Ans: Select SUM(Population) from CITY where COUNTRYCODE = 'JPN' ;

2)Query the difference between the maximum and minimum populations in CITY.

Ans: Select MAX(Population) - MIN(Population) from City;

3)Write a query that prints a list of employee names (i.e.: the name attribute) for employees in Employee having a salary greater than  per month who have been employees for less than  months. Sort your result by ascending employee_id.

Ans: Select name from Employee
where salary > 2000 and months < 10 
order by employee_id;

4)Write a query that prints a list of employee names (i.e.: the name attribute) from the Employee table in alphabetical order.

Ans: select name from employee order by name;

5)Query the list of CITY names from STATION that either do not start with vowels or do not end with vowels. Your result cannot contain duplicates.

Ans: Select DISTINCT City from Station where city not like "[aeiou]%" or city not like "%[aeiou]";









