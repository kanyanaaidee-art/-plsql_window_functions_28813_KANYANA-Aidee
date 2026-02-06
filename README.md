# plsql_window_functions_28813_KANYANA-Aidee
## Project Overview

A comprehensive implementation of SQL window functions for healthcare analytics, featuring patient service analysis, billing trends, and resource planning metrics using Oracle SQL. This academic project demonstrates practical applications of analytical SQL for healthcare department intelligence.

## A. Problem Definition

1. Organization: HealthCare Organization
2. Department:Health Services Department

Business Challenge:
The health department needs to analyze patient service records and billing data to identify the most frequently used services, track service trends over time, and segment patients for better resource allocation and service planning. Currently, they lack clear insights from their data.

Expected Outcome:
Data-driven decisions for resource allocation, service improvement, and patient segmentation based on quantitative analysis of patient visits and billing patterns.



## B. Database Schema

The database contains three related tables:

1. patients

* patient_id
* patient_name
* region

2. services

* service_id
* service_name
* service_cost

3. transactions

* transaction_id
* patient_id
* service_id
* service_date

It also contains an **ER Diagram** (see attached screenshot).



## Window Functions Implemented

1. RANK():
Shows the top services used by patients.
Interpretation: Helps identify which services are most popular among patients.

2. SUM() OVER():
Runs monthly billing totals.
Interpretation: Shows cumulative billing per month, helping track overall revenue and patient service usage.

3. LAG()/LEAD():
Month-over-month growth.
Interpretation: Helps see if patient visits or billing amounts are increasing or decreasing month-to-month.

4. NTILE(4):
Patient quartiles.
Interpretation: Segments patients into quartiles based on spending or service usage, identifying high-value patients and low-frequency patients.

5. AVG() OVER():
Three-month moving averages.
Interpretation: Smooths short-term fluctuations in service usage or billing to reveal underlying trends.



## Result Analysis

1. Descriptive (What Happened):

* General Checkups and Blood Tests are the most used services.
* January and March had the highest patient visits.

2. Diagnostic (Why It Happened):

* General Checkups are routine services and attract many patients.
* Seasonal health campaigns and patient awareness increase visits in January and March.

3. Prescriptive (What To Do Next):

* Ensure sufficient staff and resources for high-demand services.
* Promote lesser-used services to balance workload and improve service coverage.
* Monitor patient trends to optimize scheduling and inventory of medical supplies.

## Documentation
## Database Design
The database consists of three main tables:
* Patients: Stores patient identification and regional information.
* Services: Stores healthcare service details and costs.
* Transactions: Stores records of services provided to patients and billing amounts.
* Primary and foreign keys were used to maintain data integrity and relationships between tables.

## References

1. Oracle SQL Documentation: [https://docs.oracle.com/en/database/oracle/oracle-database/](https://docs.oracle.com/en/database/oracle/oracle-database/)
2. SQL Window Functions Tutorial: [https://www.w3schools.com/sql/sql_func_over.asp](https://www.w3schools.com/sql/sql_func_over.asp)
3. DB Design & ER Diagram Guide: [https://dbdiagram.io](https://dbdiagram.io)
4. Provost, F., & Fawcett, T. (2013) - Data Science for Business. O'Reilly Media.

Integrity Statement:

> “All sources were properly cited. Implementations and analysis represent original work. No AI-generated content was copied without attribution or adaptation.”
