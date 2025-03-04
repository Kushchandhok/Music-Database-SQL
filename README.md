# 🎵 Music Database Analysis (PostgreSQL)  

This project explores a **music streaming database** to analyze key business metrics such as **top customers, best-performing artists, song lengths, revenue distribution, and top genres** using SQL.  

## 📌 Key Insights & Queries  
Some of the key questions answered in this analysis:  
- 💰 **Who are the highest-spending customers?**  
- 🎤 **Which artists have the most played songs?**  
- 🎵 **What are the top music genres?**  
- 💳 **How much has each customer spent on different artists?**

### 📝 Sample SQL Query: Who is the best customer? The customer who has spent the most money will be declared the best customer. Write a query that returns te customer who has spent the most?

select customer.customer_id, customer.first_name, customer.last_name, sum(invoice.total) as total
from customer
join invoice on customer.customer_id = invoice.customer_id
group by customer.customer_id
order by total desc
limit 1;

(More queries available in the full document.)

**Technologies Used
Database: PostgreSQL
SQL Concepts: JOIN, GROUP BY, ORDER BY, LIMIT, WITH RECURSIVE, HAVING, WHERE, CASE, CTE
Documentation: MS Word**

[sql project music database.docx](https://github.com/user-attachments/files/19072731/sql.project.music.database.docx)


   
