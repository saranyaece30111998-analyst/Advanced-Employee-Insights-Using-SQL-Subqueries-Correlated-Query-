
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
   

2. Employees who earn more than Ravi.  
   ```sql
   SELECT empname
   FROM employees
   WHERE salary > (SELECT salary FROM employees WHERE empname='Ravi');
   ```
    

3. Employees who joined after Meena.  
   ```sql
   SELECT empname, joindate
   FROM employees
   WHERE joindate > (SELECT joindate FROM employees WHERE empname='Meena');
   ```

4. Employees whose salary is greater than the average salary of the IT department.  
   

5. Employees whose performance rating is higher than the company average.  
   

---

### 🔹 Multi-Row Subqueries
6. Employees who work in departments located in Chennai or Bangalore.  
   

7. Employees who work in departments located in Pune.  
   

8. Employees whose salary is greater than any employee in Marketing.  
   

9. Employees whose salary is greater than all employees in HR.  
    

10. Employees in departments with performance rating = 5.  
     

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
   `[Looks like the result wasn't safe to show. Let's switch things up and try something else!]`

20. Employees whose salary is greater than the average salary of employees who joined after them.  
   `[Looks like the result wasn't safe to show. Let's switch things up and try something else!]`

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

---

## 📸 Screenshots
All query outputs are documented with screenshots for clarity.  
Place your screenshots in a `screenshots/` folder and link them as shown above.

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

---

✨ This README is structured, professional, and recruiter-friendly. You just need to **replace the placeholders (`screenshots/...`) with your actual screenshot file paths**.  

Would you like me to also create a **GitHub profile README template** that highlights your skills and projects (like this one) for recruiters?
