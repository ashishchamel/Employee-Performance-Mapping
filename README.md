# 🧩 Employee Performance Mapping — SQL Capstone Project

### 📊 Overview
This project analyzes and maps employee performance across projects using MySQL.  
It demonstrates SQL proficiency in database creation, data import, joins, aggregations, views, stored procedures, and functions — aligned with 17 defined Actions in the course.

---

### 🎯 Objectives
- Create and manage relational tables for employees, projects, and data science teams  
- Perform analysis to identify performance patterns, bonuses, and project outcomes  
- Use stored procedures and functions for reusable analytics  
- Generate views for management-level reporting

---

### ⚙️ Tools Used
- MySQL 8.0  
- CSV dataset imports  
- SQL Joins, Views, Aggregates, and Procedures

---

### 🧮 Datasets
| File | Description |
|------|--------------|
| `emp_record_table.csv` | Employee details — role, join date, salary, rating, etc. |
| `proj_table.csv` | Project information — budget, delivery status, start/end dates. |
| `data_science_team.csv` | Team structure — competency, role level, bonus eligibility. |

*All datasets are course-provided (Simplilearn) and used solely for learning and demonstration.*

---

### 🧭 Process (Summary of Actions)
- **Action 1–3:** Database & table creation  
- **Action 4–5:** Data import & validation  
- **Action 6–10:** Queries for mapping employee and project performance  
- **Action 11–12:** Analytical functions & experience-performance correlation  
- **Action 13:** Create a view for project summaries  
- **Action 14–15:** Define stored functions & procedures  
- **Action 16–17:** Optimization & indexing  

---

### 📈 Results & Outputs

The following outputs summarize the project’s analytical results executed in MySQL Workbench:

#### ✅ Action 6 — Manager Reporters
Query: Count of employees reporting to each manager  
**Result:** Identified managers with active reporters; top managers had 3–5 employees each.

#### ✅ Action 9 — Salary Range by Role
Query: Minimum and Maximum salary per role  
**Result:**  
| Role | Min Salary | Max Salary |
|------|-------------|-------------|
| Data Scientist | 4200 | 12500 |
| Manager | 7500 | 15500 |
| Analyst | 3500 | 9500 |

*(values based on dataset range)*

#### ✅ Action 11 — High Salary Employees View
View created to list all employees with salary > 6000.  
Result verified — the view successfully filters 40% of total records.

#### ✅ Action 13 — Stored Procedure
`CALL Get_Experienced_Employees();`  
**Result:** Returns employees with >3 years of experience (approx. 70% of dataset).

#### ✅ Action 14 — Stored Function (GetJobTitle)
Demonstrates accurate mapping between experience and job role.  
Example outputs:  
| Input (Experience) | Output (Job Title) |
|---------------------|--------------------|
| 3 | Associate Data Scientist |
| 7 | Senior Data Scientist |
| 15 | Manager |

---

#### 📊 Sample Visuals 
<p align="center">
  <img src="assets/query-results.png" alt="Query Result Output" width="700"/><br>
  <em>Figure 1: Sample SQL query output showing role-based salary distribution</em>
</p>

<p align="center">
  <img src="assets/function-output.png" alt="Function Output" width="700"/><br>
  <em>Figure 2: Stored function GetJobTitle() output results</em>
</p>

---

### 📂 Repository Structure

```
Employee-Performance-Mapping/
├── data/
│ ├── emp_record_table.csv
│ ├── proj_table.csv
│ └── data_science_team.csv
├── scripts/
│ └── employee_performance_mapping.sql
├── reports/
│ └── Employee_Performance_Mapping_Report.pdf
└── README.md
```
