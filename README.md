# 📚 Library Management System — SQL & Power BI Project

## 🧩 Project Overview
The **Library Management System** is a data-driven project that integrates **SQL database design** and **Power BI visualization** to manage and analyze library operations efficiently.  
It demonstrates end-to-end data handling — from database creation and normalization in **MySQL** to business insights visualization in **Power BI**.

This project is built to highlight expertise in **database design, SQL queries, data relationships, and reporting dashboards**, making it ideal for showcasing technical and analytical skills to recruiters.

---

## ⚙️ Key Features

### 🗄️ SQL Database Design
- Normalized relational database for managing **books, customers, employees, branches, and transactions**.
- Enforced **primary and foreign key constraints** to maintain referential integrity.
- Populated with realistic sample data for queries and analysis.

### 🧠 Data Analysis using SQL
Includes optimized SQL queries for:
- Retrieving available books and rental details.
- Calculating employee salary insights.
- Identifying active customers and branch statistics.
- Generating category-based book counts.
- Performing joins, groupings, subqueries, and aggregations for business insights.

### 📊 Power BI Dashboard
The **Power BI report (`Library project.pbix`)** connects to the SQL dataset to deliver:
- KPIs for **total books, borrowed books, active customers**, and **branch performance**.
- Interactive charts for **book categories, rental trends**, and **employee analysis**.
- Filters for exploring **branches**, **authors**, or **customers** dynamically.

---


---

## 🧮 Database Schema

### Core Tables
| Table | Description |
|--------|-------------|
| **Branch** | Stores branch details and manager info |
| **Employee** | Tracks employee data with salary and branch assignment |
| **Customer** | Contains customer registration and address info |
| **Books** | Catalog of all library books with rental status |
| **IssueStatus** | Records of issued books |
| **ReturnStatus** | Records of returned books |

---

## 🧾 Sample Analytical Queries
| Query | Description |
|--------|-------------|
| Retrieve available books | `SELECT Book_title, Category, Rental_Price FROM Books WHERE Status='Yes';` |
| Employees earning above ₹50,000 | `SELECT Emp_name, Position FROM Employee WHERE Salary > 50000;` |
| Books issued by customers in May 2023 | `SELECT Customer_name FROM Customer INNER JOIN IssueStatus ...;` |
| Count of books by category | `SELECT Category, COUNT(*) FROM Books GROUP BY Category;` |
| Branches with >2 employees | `SELECT Branch_no, COUNT(Emp_id) FROM Employee GROUP BY Branch_no HAVING COUNT(Emp_id)>2;` |

---

## 📈 Power BI Dashboard Highlights
- **KPI Cards:** Total Books, Issued Books, Active Customers, Total Employees.  
- **Visuals:**  
  - Bar chart: Books by Category  
  - Pie chart: Issued vs Returned books  
  - Matrix: Employee Salaries by Branch  
  - Line chart: Monthly issue trends  
- **Filters & Slicers:** Region, Category, Branch, Author.

---

## 🧰 Tools & Technologies
| Tool | Purpose |
|------|----------|
| **MySQL / SQL** | Database creation, data manipulation & queries |
| **Power BI** | Visualization and reporting |
| **DAX** | Power BI measures & KPIs |
| **Data Modeling** | Establishing relationships between entities |

---

## 🚀 How to Use
1. Import the SQL file into **MySQL Workbench** or any SQL client.
2. Execute the script to create all tables and insert data.
3. Open the **Power BI (.pbix)** file and connect it to your local database.
4. Create visual analytical dashboard.

---

## 💡 Insights
- Identified **top borrowed book categories** (Classics, History, Fantasy).  
- Recognized **most active branches** based on book issues.  
- Analyzed **employee salary distribution** and **customer engagement** trends.  
- Highlighted **inventory turnover rate** for popular books.

---

## 🔮 Future Enhancements
- Integrate **real-time SQL connection** for auto-refresh dashboards.  
- Add **return delay penalties** and **fine calculations** in SQL logic.  
- Build a **frontend web interface** for live library management.

---

## 👩‍💻 Author
**Ayesha Bathool**  
Aspiring Data Analyst | SQL Developer | Power BI Enthusiast | MIS Executive

📧 Email: ayeshabathool14@gmail.com 
🔗 LinkedIn: www.linkedin.com/in/ayesha-bathool-b05b35292  
💾 GitHub: https://github.com/ayeshabathool14?tab=repositories

---

## 🏷️ Tags
`#SQLProject` `#PowerBI` `#DataAnalytics` `#LibraryManagementSystem` `#DatabaseDesign` `#DataVisualization`



