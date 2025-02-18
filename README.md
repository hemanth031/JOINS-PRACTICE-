# JOINS-PRACTICE-
-- INNER JOIN (only matching records)
SELECT e.emp_id, e.name, d.dept_name 
FROM Employees e
INNER JOIN Departments d ON e.dept_id = d.dept_id;

-- LEFT JOIN (all from Employees, matching from Departments)
SELECT e.emp_id, e.name, d.dept_name 
FROM Employees e
LEFT JOIN Departments d ON e.dept_id = d.dept_id;

-- RIGHT JOIN (all from Departments, matching from Employees)
SELECT e.emp_id, e.name, d.dept_name 
FROM Employees e
RIGHT JOIN Departments d ON e.dept_id = d.dept_id;

-- FULL JOIN (all records from both tables)
SELECT e.emp_id, e.name, d.dept_name 
FROM Employees e
FULL JOIN Departments d ON e.dept_id = d.dept_id;
