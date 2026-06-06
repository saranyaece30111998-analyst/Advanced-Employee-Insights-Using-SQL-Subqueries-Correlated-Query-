
# Advanced Employee Insights Using SQL – Subqueries & Correlated Queries

## 📌 Project Overview
This project demonstrates the use of **SQL subqueries** and **correlated subqueries** to analyze employee and department data in the `CompanyDB` database.  
It covers salary benchmarking, performance evaluation, and departmental analysis — essential skills for HR analytics and business intelligence.

---

## 📂 Table of Contents
1. Introduction  
2. Methodology  
   - Single-Row Subqueries  
   - Multi-Row Subqueries  
   - Correlated Subqueries  
3. Results  
4. Conclusion  
5. Screenshots  

---

## 1️⃣ Introduction
The goal of this project is to strengthen query-writing skills and apply them to real-world HR and business scenarios.

---

## 2️⃣ Methodology

### 🔹 Single-Row Subqueries
1. Employees whose salary is greater than the average salary of all employees.  
   ```sql
   SELECT empname
   FROM employees
   WHERE salary > (SELECT AVG(salary) FROM employees);
   ```
   <img width="643" height="315" alt="Screenshot 2026-06-05 174752" src="https://github.com/user-attachments/assets/d968230c-18ca-43a3-b5ba-448912efe1cd" />


2. Employees who earn more than Ravi.  
   ```sql
   SELECT empname
   FROM employees
   WHERE salary > (SELECT salary FROM employees WHERE empname='Ravi');
   ```
    <img width="597" height="470" alt="Screenshot 2026-06-05 175224" src="https://github.com/user-attachments/assets/d9b5f6e2-b450-4d31-ad48-55c513cdcb0e" />


3. Employees who joined after Meena.  
   ```sql
   SELECT empname, joindate
   FROM employees
   WHERE joindate > (SELECT joindate FROM employees WHERE empname='Meena');
   ```
<img width="652" height="457" alt="Screenshot 2026-06-05 175447" src="https://github.com/user-attachments/assets/d2c82c2d-5ce1-4238-a1ab-2bfda8a26f54" />

4. Employees whose salary is greater than the average salary of the IT department.  
   <img width="1013" height="423" alt="Screenshot 2026-06-05 175824" src="https://github.com/user-attachments/assets/69da26a2-a3d5-46e8-92a3-181f878d7368" />


5. Employees whose performance rating is higher than the company average.  
   
<img width="1032" height="521" alt="Screenshot 2026-06-05 180322" src="https://github.com/user-attachments/assets/2ef65ea8-76c8-4ee0-b296-499e82f6c38f" />

---

### 🔹 Multi-Row Subqueries
6. Employees who work in departments located in Chennai or Bangalore.  
   <img width="773" height="617" alt="Screenshot 2026-06-05 190238" src="https://github.com/user-attachments/assets/2eba0310-9f9e-45b3-8bd8-c5ceb60a4fc1" />


7. Employees who work in departments located in Pune.
   
 -<img width="466" height="457" alt="Screenshot 2026-06-05 190657" src="https://github.com/user-attachments/assets/d89c6dc8-3090-4238-9015-fd8cf2bba703" />

   

9. Employees whose salary is greater than any employee in Marketing.  
   <img width="908" height="507" alt="Screenshot 2026-06-05 183147" src="https://github.com/user-attachments/assets/f0709411-d077-4ce7-a086-b36c6b2209a4" />


10. Employees whose salary is greater than all employees in HR.  
    

11. Employees in departments with performance rating = 5.  
     

---

### 🔹 Correlated Subqueries
11. Employees whose salary is greater than the average salary of their department.  


12. Employees who earn the highest salary in their department.  
    

13. Employees whose performance rating is higher than their department average.  
    

14. Employees who joined after the average join date of their department.  
    

15. Employees whose salary is less than the maximum salary in their department.  
    

16. Employees whose salary is equal to the minimum salary in their department.  
    

17. Departments that have employees earning more than 70,000.  
     

18. Employees whose salary is greater than at least one employee in their department.  
    

19. Employees who are the only employee in their department.  
    

20. Employees whose salary is greater than the average salary of employees who joined after them.  
     

---

## 3️⃣ Results
- **Salary Analysis**: Identified employees above average, top earners, and those below departmental maximums.  
- **Performance Insights**: Highlighted employees outperforming both company-wide and departmental averages.  
- **Departmental Trends**: Located employees based on city-specific departments and salary thresholds.  
- **Unique Cases**: Found single-employee departments and employees joining after departmental averages.  

---

## 4️⃣ Conclusion
This project provides a comprehensive practice set for SQL subqueries.  
By covering single-row, multi-row, and correlated subqueries, it equips learners with the ability to answer complex business questions.  
These queries form the foundation for **business intelligence reporting** and **data-driven decision-making**.

--


---

## 🛠️ Tech Stack
- SQL (MySQL / PostgreSQL compatible)  
- CompanyDB dataset  

---

## 👩‍💻 Author
**Saranya** – Engineering Graduate & Data Analyst  
Skilled in Power BI, SQL, Python, Excel  
📍 India  

```



