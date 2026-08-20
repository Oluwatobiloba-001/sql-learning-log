# Day 2: WHERE & ORDER BY

**Date**: Aug 21, 2026
**Learning from**: Alex The Analyst YouTube Channel

## What I Learned Today

Today I learned how to FILTER and SORT data using `WHERE` and `ORDER BY`.

### 1. `WHERE` - To filter rows
This lets me get only the data I want, like Excel filters.

```sql
-- Find employees older than 40
SELECT first_name, last_name, age
FROM packs_and_recreation.employee_demographics
WHERE age > 40;

-- Find employees who are NOT in Sales
SELECT *
FROM packs_and_recreation.employee_demographics
WHERE department != 'Sales';

-- Find employees born after 1990
SELECT first_name, birth_date
FROM packs_and_recreation.employee_demographics
WHERE birth_date > '1990-01-01';

Filtering with dates
-- Show people born after 1985
SELECT *
FROM employee_demographics
WHERE birth_date > '1985-01-01';

Logical operators: AND,OR,NOT
-- AND: Born after 1985 AND Male
SELECT *
FROM employee_demographics
WHERE birth_date > '1985-01-01'
AND gender = 'Male';

-- OR: Born after 1985 OR Male
SELECT *
FROM employee_demographics
WHERE birth_date > '1985-01-01'
OR gender = 'Male';

-- NOT: Born after 1985 AND NOT Male = Females
SELECT *
FROM employee_demographics
WHERE birth_date > '1985-01-01'
AND NOT gender = 'Male';

LIKE operator
-- Show everyone whose first name starts with 'Jer'
SELECT *
FROM employee_demographics
WHERE first_name LIKE 'Jer%'Jer

Key
