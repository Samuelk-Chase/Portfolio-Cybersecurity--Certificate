# Apply Filters to SQL Queries

## Project Description

This project demonstrates how to apply filters to SQL queries to retrieve specific information from a database. It covers retrieving after-hours failed login attempts, login attempts on specific dates, login attempts outside of a specific location, retrieving employees in specific departments, and filtering employees based on department membership.

## Retrieve After-Hours Failed Login Attempts

```sql
SELECT *
FROM login_attempts
WHERE login_timestamp BETWEEN 'after_hours_start_time' AND 'after_hours_end_time'
AND login_outcome = 'failed';
```

## Retrieve Login Attempts on Specific Dates

```sql
SELECT *
FROM login_attempts
WHERE DATE(login_timestamp) = 'specific_date';
```

## Retrieve Login Attempts Outside of Mexico

```sql
SELECT *
FROM login_attempts
WHERE login_location != 'Mexico';
```

## Retrieve Employees in Marketing

```sql
SELECT *
FROM employees
WHERE department = 'Marketing';
```

## Retrieve Employees in Finance or Sales

```sql
SELECT *
FROM employees
WHERE department IN ('Finance', 'Sales');
```

## Retrieve All Employees Not in IT

```sql
SELECT *
FROM employees
WHERE department != 'IT';
```

## Summary

This file provides a brief overview of applying filters to SQL queries to retrieve specific information from a database. Refer to the specific sections for detailed SQL queries and examples.
