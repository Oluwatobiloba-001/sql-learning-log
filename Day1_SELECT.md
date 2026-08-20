# Day 1: SELECT Statement

**Date**: Aug 20, 2026
**Learning from**: Alex The Analyst YouTube Channel

## What I Learned Today

Today I learned the `SELECT` statement. This is how we pull data from tables in SQL.

### 1. I learnt how to select a single column
```sql
SELECT first_name
FROM packs_and_recreation.employee_demographics;

###2. I learnt how to select multiple columns
```sql
SELECT first_name, last_name, birth_date
FROM packs_and_recreation.employee_demographics;

###3. I learnt how to make calculations 
SELECT first_name, 
       last_name, 
       birth_date, 
       age,
       age + 10
FROM packs_and_recreation.employee_demographics;

Learning SQL in public
#DaysOfSQL #SQL #Data Analysis #AlexTheAnalyst
