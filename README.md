## Overview

This repository contains a detailed security investigation using SQL filters to examine suspicious login activity and employee data. The project simulates a real-world scenario where a security professional uses structured queries to identify potential threats within an organization's infrastructure.

The purpose of this project is to showcase practical SQL filtering techniques that support identifying, analyzing, and responding to cybersecurity incidents related to unauthorized access attempts and internal asset exposure.

---

## Activity Summary

The project involved analyzing the `log_in_attempts` and `employees` tables to uncover signs of potential misuse or compromise. The main objectives were:

- Investigate failed login attempts occurring outside business hours.
- Filter login attempts on critical incident dates.
- Detect access attempts originating from outside of Mexico.
- Identify employees in specific departments and locations for targeted response.
- Exclude unaffected departments to focus security efforts where needed.

---

## Scenario

You are a security professional at a large organization. Recently, your team discovered suspicious login activity outside of business hours. You were assigned to investigate using the organization’s SQL-accessible logs and employee directory.

The analysis involved:
- Investigating failed login attempts after 6:00 PM.
- Examining logins on the incident date (2022-05-09) and the day before.
- Identifying login attempts that did **not** originate in Mexico.
- Filtering employees based on department (Marketing, Finance, Sales) and location (East building).
- Excluding the IT department from remediation efforts due to prior updates.

To carry out the investigation, SQL filters were used to extract, refine, and analyze relevant records from the database.

---

## Key Steps

- Queried failed login attempts after 18:00 hours to detect after-hours activity.
- Used date filtering to identify login attempts around the time of the incident.
- Applied `NOT LIKE` pattern matching to isolate login attempts from outside Mexico.
- Retrieved employee information based on department and office filters.
- Used `NOT` conditions to exclude IT staff from certain updates.

---

## Tools and Methods Used

- **SQL Filtering Techniques**: Used `WHERE`, `AND`, `OR`, `NOT`, `LIKE`, and time/date filters
- **Database Tables**: `log_in_attempts`, `employees`
- **Logical Filtering**: Applied conditional logic to isolate specific data patterns

---

## Project Files

- **SQL Scripts**: [Apply filters to SQL queries](./Apply%20filters%20to%20SQL%20queries.pdf)

---