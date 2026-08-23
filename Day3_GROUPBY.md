# Day 3: GROUP BY + Aggregate Functions

**Date**: Aug 22, 2026
**Learning from**: Alex The Analyst YouTube Channel

## What I Learned Today

Today I learned how to GROUP and SUMMARIZE data using `GROUP BY` with aggregate functions. 
This is like Excel Pivot Table.

### 1. Basic `GROUP BY`
Groups rows that have the same values.
```sql
-- Count how many employees in each gender
SELECT gender
FROM employee_demographics
GROUP BY gender;

-- Count how many employees in each gender
SELECT gender, COUNT(age) AS total_employees
FROM employee_demographics
GROUP BY gender;

-- Count how many employees in each occupation
SELECT occupation, COUNT(*) AS total_employees
FROM employee_salary
GROUP BY occupation;

-- Find average, min, and max age for each gender
SELECT 
    gender,
    AVG(age) AS average_age,
    MIN(age) AS youngest_age,
    MAX(age) AS oldest_age,
    COUNT(age) AS total_people
FROM employee_demographics
GROUP BY gender;

GROUP BY multiple columns
-- Group by both occupation AND salary
SELECT occupation, salary, COUNT(*) AS total_employees
FROM employee_salary
GROUP BY occupation, salary
ORDER BY occupation;


Key things I learnt

 1.  *`GROUP BY`*: Groups rows together. Always comes AFTER `WHERE`
2.  *Aggregate Functions*: `COUNT()`, `AVG()`, `MIN()`, `MAX()`, `SUM()`

0 likes on Day 1. Still posting on Day 3

 Learning SQL in public with #TheStatsLady #SQL #DataAnalytics #AlexTheAnalyst
