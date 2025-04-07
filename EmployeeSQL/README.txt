# Module 9: SQL Challenge - Pewlett Hackard Employee Database 

## 📋 Chellenge Overview

This challenge is showcases data modeling, engineering, and analysis using historical employee data from a fictional company called "Pewlett Hackard".

The objectives were:
- Data Modeling: Design a relational database schema
- Data Engineering: Import CSV files into PostgreSQL
- Data Analysis: Run SQL queries to analyze employee


The following were used:
- PostgreSQL
- pgAdmin
- SQL
- CSV (Comma-Separated Values)
- Git + GitHub
- QuickDBD

---

## 🗂️ Challenge File Structure

sql challenge/
├── EmployeeSQL/
│   ├── data/                     # Original CSV files
│   ├── Tables_Creation.sql      # Code to create tables
│   ├── Queries.sql              # 8 assignment queries
│   ├── employees_db_schema.png  # Screenshot of Entity Relationship Diagram of the tables
│   └── README.md                # Summary of the challenge


---

## 🧱 Database Design

The database includes six tables:
- 'employees': Basic employee details
- 'departments': List of departments
- 'titles': Job titles
- 'salaries': Employee salary records
- 'dept_emp': Employee and their corresponding departments
- 'dept_manager': Departments and their corresponding managers

Entity relationships were modeled using primary and foreign keys, with composite keys in `dept_emp` and `dept_manager`.

---

## 📥 Data Import Process

- Created tables in PostgreSQL using 'Tables_Creation.sql'
- Imported CSVs using pgAdmin’s "Import Tool" in the following order:
  1. 'titles'
  2. 'departments'
  3. 'employees'
  4. 'salaries'
  5. 'dept_emp'
  6. 'dept_manager'

Common errors resolved:
- Foreign key errors (due to incorrect import order)
- Column mismatch and type errors (resolved by checking column order before import)


---

## 🔍 Data Analysis Queries

Eight analysis queries were completed in 'Queries.sql'. They are:
1. List the employee number, last name, first name, sex, and salary of each employee.
2. List the first name, last name, and hire date for the employees who were hired in 1986.
3. List the manager of each department along with their department number, department name, employee number, last name, and first name.
4. List the department number for each employee along with that employee’s employee number, last name, first name, and department name.
5. List first name, last name, and sex of each employee whose first name is Hercules and whose last name begins with the letter B.
6. List each employee in the Sales department, including their employee number, last name, and first name.
7. List each employee in the Sales and Development departments, including their employee number, last name, first name, and department name.
8. List the frequency counts, in descending order, of all the employee last names (that is, how many employees share each last name).

---

## 🚀 How to Run

1. Open pgAdmin and create a new database e.g. 'employee_db'
2. Execute 'Tables_Creation.sql' in the Query Tool of pgAdmin to create the tables
3. Use pgAdmin’s Import Tool to load the CSVs from the 'data' folder (in the correct order)
4. Open and execute 'Queries.sql' to run the challenge queries

---

## 📌 Notes

This challenge was part of a SQL-focused challenge designed to simulate real-world data engineering and analysis tasks. It demonstrates proficiency in:
- Schema design and normalization
- Data integrity with primary/foreign keys
- Querying with joins, filters, and aggregation
