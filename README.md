Overview

This project implements a modern Data Engineering platform that consolidates data from multiple sources into a centralized, analytics-ready data warehouse. The solution follows industry-standard ELT practices and demonstrates how organizations create a reliable "Single Source of Truth" for reporting and decision-making.

The platform ingests data from APIs, CSV files, and relational databases, stores raw data in a cloud-based data lake, performs transformations using dbt, orchestrates workflows with Apache Airflow, validates data quality using automated tests, and delivers insights through interactive dashboards.

Key Features
Multi-source data ingestion (REST APIs, CSV files, MySQL)
Cloud-based Data Lake on Google Cloud Storage (GCS)
Workflow orchestration using Apache Airflow
Data transformation and modeling using dbt
Star Schema implementation for analytics
Automated data quality checks with dbt tests and Great Expectations
BigQuery Data Warehouse for scalable analytics
Interactive dashboards using Looker Studio
Dockerized deployment for reproducibility
Architecture
Plain Text
1
API + CSV + MySQL
2
|
3
v
4
Google Cloud Storage (Data Lake)
5
|
6
v
7
Apache Airflow
8
|
9
v
10
dbt Transformations
11
|
12
v
13
BigQuery Data Warehouse
14
|
15
+--> Data Quality Checks
16
|
17
v
18
Looker Studio Dashboard
Show more lines
Tech Stack
Python
SQL
Apache Airflow
dbt
Google Cloud Storage (GCS)
BigQuery
Great Expectations
Docker
Looker Studio
Git & GitHub
Business Problem

Organizations often collect data from multiple disconnected systems, resulting in inconsistent reporting and duplicated metrics. This project addresses that challenge by creating a centralized data platform that provides a trusted source of business information for analytics and decision-making.

Data Pipeline Workflow
Extract data from APIs, CSV files, and MySQL databases.
Store raw data in Google Cloud Storage.
Schedule and monitor workflows using Airflow.
Transform and model data using dbt.
Load curated datasets into BigQuery.
Execute automated data quality checks.
Build dashboards for business reporting and KPI tracking.
Outcomes
Unified data from multiple sources into a centralized analytics platform.
Automated end-to-end ELT workflow with minimal manual intervention.
Improved data reliability through automated validation checks.
Designed scalable warehouse architecture using star schema modeling.
Enabled real-time business insights through dashboard reporting.
