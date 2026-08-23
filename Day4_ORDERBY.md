# Day 4: ORDER BY - Sorting Data

**Date**: Aug 23, 2026
**Learning from**: Alex The Analyst YouTube Channel

## What I Learned Today

Today I learned how to SORT results using `ORDER BY`. 
This is like clicking "Sort A-Z" in Excel.

### 1. `ORDER BY` Ascending - A to Z, 1 to 9
Default is ASC so you don't always need to write it.
```sql
-- Sort employees by first name A to Z
SELECT *
FROM employee_demographics
ORDER BY first_name ASC;

-- Same as above, ASC is default
SELECT *
FROM employee_demographics
ORDER BY first_name;

ORDER BY descending order
-- Sort employees by first name Z to A
SELECT *
FROM employee_demographics
ORDER BY first_name DESC;


--ORDER BY MULTIPLE COLUMNS
-- First sort by gender A-Z, then sort age from youngest to oldest
SELECT *
FROM employee_demographics
ORDER BY gender, age;

-- First sort by gender, then sort age from oldest to youngest
SELECT *
FROM employee_demographics
ORDER BY gender, age DESC;



Key Things I Learned:
1.  *`ORDER BY`*: Sorts your results. Always comes LAST in a query
2.  *`ASC`*: Ascending. A-Z, 1-9. This is default
3.  *`DESC`*: Descending. Z-A, 9-1
4.  *Multiple columns*: `ORDER BY gender, age` = sort by gender first, then age


Learning SQL in public with #TheStatsLady #SQL #DataAnalytics #AlexTheAnalystnding
