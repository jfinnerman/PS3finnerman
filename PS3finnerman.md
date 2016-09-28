# PS3finnerman
## Problem Set 3 

1. Define the terms: relation, tuple, attribute, record, and field.
  
  Relation: a set of tables
  
  Tuple:a record or row
  
  Attribute: a column or field
  
  Record:is also known as a tuple or row, it represents a structured data item in a table
  
  Field: also known as an attribute or column, an example of a field is a category in a column like weight, height, price, or manufacturer_id. 
  
2. What are keys in a relation?

  Keys link a relation. Each table in the relation has a primary key which uniquely identifies tuples, or records, in that table. Some tables also contain foreign keys which indicates a relationship between tables. 

3. What is a surrogate key and how is it used?

  A surrogate key is a unique key which is an identifier for an record in a relation. A surrogate key can be a primary key. It is a system generated key and is factless.

4. In the following equation, Area = Length x Width, identify the determinant(s).

  Length and Width

5. If a relation has no duplicate data, how can you be sure there is always at least one primary key?

  You can add a foreign key to the table which then creates duplicate data.

6. Give an example of a relation.  Determine a natural key for this relation.

  An example of a relation is an employee's personal information. A natural key for this relation would be the employees social security number.

  For question 7 - 8, Consider product *orders*.  In particular, associated with an order is: customer name (first and last), address (street, city, state, zip), phone, email, the products orders (including item, quantity, and price).  

7. Create a relational data model for *orders*.  Consider applying normalization rules (discuss Monday)

8. For customer, could email be used as a primary key?  If so, state why.  Also, if possible to use as a primary key, discuss any disadvantages of using email as a primary key.
  
  It is possible as long as each customer has an email address but it would not work if not all customers listed one. There are multiple disadvantages if using an email as a primary key. One disadvantage is that you store the email address multiple times. Another disadvantage is that emails, like phone numbers, sometimes change. So one year, someone could have that email but get a new one the next year. Also, that old email address could be taken over by another person which is not a good thing because you could then be sending confidential or unwanted information to a random person. Also, since emails change frequently, if you are joining to other tables with that as the key, then you will have to update the other tables as well which can takes a lot of time especially when an entire client company changes their emails.
  
9. Given two relations S and R below find the Cartsian Product S x R. 

  Every element of S has to be matched to R. (1,2,3,1,1,1,2,2,2,3,1,2,2,1,5,2,3,3,1,1,2,3,2,2,3,2,3,2,1,5)
  
10. Find the natural join between the Faculty and Department relations below.

  The natural join is Department.
  
S
--------------
| A | B |
|---|---|
| 1 | 2 |
| 2 | 3 |
---------

R
------------
| C | D | E |
|---|---|---|
| 3 | 1 | 1 |
| 2 | 2 | 3 |
| 2 | 1 | 5 |



Faculty
--------------
| Name | ID | Dept |
|-------|----|----------------|
| Joe | 1 | Chemistry |
| Susan | 2 | Math |
| Tom | 3 | Marine Science |
| Mike | 4 | Math |


Department
------------
| Dept | Chair  |
|---|---|
| Chemistry | John |
| Math | Mike |
| Marine Science | Barry |
