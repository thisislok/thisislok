# 🏢 Model-a-Company - SQL Business Database

### 💡 Practical Challenge: SQL Schema Design & Reporting

## 📄 Description  
This project models a fictional company's internal database system using **relational SQL**.  
It demonstrates how to design and query tables such as **employees**, **customers**, **products**, and **orders**.  
Key goals include linking tables via **foreign keys**, performing **aggregated calculations**, and generating **real-world reports** like employee commissions, customer spending, and shipping labels.

---

## 🛠️ Languages and Tools Used

- **SQL (PostgreSQL / SQLite-compatible)**
- **Entity Relationships & Joins**
- **Aggregate Functions (SUM, ROUND, GROUP BY)**

## 💻 Database Tables

- `Employees`: Stores employee info and commission rate
- `Customers`: Stores customer contact and delivery info
- `Products`: Stores items for sale
- `Orders`: Records purchases linking all three tables

---

## 🧪 Query Examples

### 📈 Total Sales Per Employee  
```sql
SELECT 
    E.FirstName || ' ' || E.LastName AS Employee,
    SUM(P.Price * O.Quantity) AS TotalSales
FROM Orders O
JOIN Employees E ON O.EmployeeID = E.EmployeeID
JOIN Products P ON O.ProductID = P.ProductID
GROUP BY E.EmployeeID;
