# codetech-sql-task1

Name: Shinde Abhishek Arvind Company: CODTECH IT SOLUTIONS ID :CT08OFK  Domain: SQL Tasks Duration: January 20th,2025 to February 20th, 2025. Mentor:Santhosh

#table description as follows:

![image](https://github.com/user-attachments/assets/48128232-4922-4c08-aba6-df08468bd362)

#left join 
*/left join to find Total revenue of products as per each category

![image](https://github.com/user-attachments/assets/27961656-792d-4f0c-9190-20f8d6c83269)

# right join 

![image](https://github.com/user-attachments/assets/031bcaa7-7040-458e-89db-c4294b5d2d13)

# full join

SELECT *
FROM customers
 JOIN sale ON customers.cust_id = sale.cust_id
 JOIN products ON sale.prod_id = products.prod_id;

 ![image](https://github.com/user-attachments/assets/1ea2af98-b82f-4f5b-a890-506e7ae79f6d)

 # inner join
 /* Assigning discount to customers according to their membership type and total 
purchase price.using case and inner join*/



select c.name, c.memb_type,s.amount,
 case
  when (s.amount>1000 and c.memb_type='bronze') then (5)
  when (s.amount>2000 and c.memb_type='silver') then(10)
  when (s.amount>3000 and c.memb_type='gold') then (15)
  when (s.amount>4000 and c.memb_type='platinum') then (20)
  else 0
   end as discount_percent
  from customers c
 inner join sale s on c.cust_id=s.cust_id;


 ![image](https://github.com/user-attachments/assets/e6cb828b-e5ae-47a7-9cfe-6655374b668b)


 Performed INNER, LEFT, RIGHT, and FULL JOINS on tables to combine data.  
- Used LEFT and RIGHT JOINs to calculate total revenue per product category.  
- Applied FULL JOIN to combine customer, sale, and product data.  
- Assigned discounts based on customer membership type and total purchase price.  
- Successfully retrieved meaningful insights using JOIN operations.  




 

 
 





