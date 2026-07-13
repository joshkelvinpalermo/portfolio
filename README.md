# Data Engineering Portfolio

Hi! My name is Josh, and I'm thrilled to share my growing professional portfolio with you. This repository contains a curated collection of projects completed through various data engineering and analytics stints, self-directed learning exercises, and company-initiated projects. Each project highlights key skills and techniques in the field.

## Company Projects

### (2025) Core Data Migration

![Core Data Migration](https://github.com/user-attachments/assets/6a0c2d6b-b9f5-46df-bee5-9a650752534d)

**DESCRIPTION**: The project aims to transition all master data processing workloads from a legacy environment, which relies on custom-built ETL pipelines for individual sub-domains, to a refreshed data mesh framework. This new framework is fully parameterized and driven entirely by JSON configurations that enables scalability and dynamic pipeline orchestration across several master data domains.

**HOW IT WORKS**: Several sub-domains contributing to the project currently export raw Parquet files on a scheduled basis. These files are then ingested by custom ETL processes, which leverage individual Databricks notebooks to perform transformations. This setup is now being modernized by consolidating into a single, unified framework that utilizes parameterized transformations driven by JSON configurations. The transformed data is subsequently exposed through views in Synapse Analytics for downstream consumption.

**TECHNOLOGY**: SAP, Azure Data Factory, Databricks, Synapse Analytics, Tableau/Power BI

---

### (2024) CleverSense

![CleverSense](https://github.com/user-attachments/assets/bd7f5eea-f044-4d4f-b7a3-5a014eb51566)

**DESCRIPTION**: This project focuses on building and maintaining an end-to-end data pipeline to collect, process, and analyze sensors, machines, and factory data from various industrial machines. The system captures real-time data from these devices, dumps them in parquet format, and is processed for analytics. Using data engineering techniques like data aggregation, transformation, and time-series analysis via Azure Databricks, the project aims to monitor machine performance, product manufacturing, and improve operational efficiency.

**HOW IT WORKS**: Several machines from the many plants and factories of the company have sensors, PLCs, and devices that generates real-time data. These raw data in the form of parquet files are ingested and stored into Data Lake, then using Databricks, these are cleaned and processed. Curated data would then be loaded into Delta Lake and is projected on Microsoft Power BI for reporting.

**TECHNOLOGY**: Azure Data Lake, Azure Data Factory, Azure Databricks, Azure Synapse Analytics, Power BI

---

### (2024) Finance Group - Global Sourcing, International Supply Chain

![Finance Group](https://github.com/user-attachments/assets/a3b61c77-f5ac-4f47-99df-af9e620d2c42)

**DESCRIPTION**: The aim of the project was to streamline the data management and analysis processes for one of the financial legs of the company. It focused on gathering, cleaning, transforming, and storing large volumes of financial data to provide actionable insights for financial analysis, forecasting, and reporting. By building a robust data pipeline and integrating various data sources, the project ensures that decision-makers have access to real-time, accurate, and comprehensive financial data.

**HOW IT WORKS**: The raw data are being extracted from SAPS4/HANA using an application built on Azure App Service, then dumped on Data Lake. Using the JSON configuration files that we developed, these data are processed and transformed based on the rules, mappings, and transformations that are defined, including the join, primary, and surrogate keys. The purpose of these JSON files were so we can just dynamically apply several transformation methods using only one framework. Cleaned and structured data would then be stored on the Delta Lake and is loaded to Tableau as the serving layer.

**TECHNOLOGY**: SAPS4/4HANA, Azure Data Lake, Azure Data Factory, Azure Databricks, Azure Synapse Analytics, Power BI

---

### (2022) STARS Stream C

![Stars Stream C](https://github.com/user-attachments/assets/b8ada157-5a17-4752-8b5b-a11a46ecc50d)

**DESCRIPTION**: The objective of this project is to migrate and modernize the bank’s legacy data warehouse infrastructure, transitioning from Cloudera-based data warehouses and on-premises mainframes to a scalable, cloud-native architecture on AWS. The project aims to reimagine how the bank stores, processes, and serves its data by leveraging AWS services for cost efficiency, elasticity, and improved performance. It involves redesigning ETL pipelines for cloud readiness, implementing data governance and security aligned with regulatory requirements, and enabling advanced analytics capabilities to support real-time insights for various banking operations.

**HOW IT WORKS**: Multiple data marts and databases previously housed in the legacy Cloudera Data Warehouse are being reconstructed on AWS Redshift. This process involves using the original Source-to-Target Mapping (STM) specifications used in their initial development to ensure consistency in data lineage and business logic during migration. Once the data warehouse is built on Redshift and the ETL pipelines on Talend, extensive validation and unit testing are performed to confirm that the data in the new environment accurately matches the legacy datasets, both in terms of data quality and business rule adherence.

**TECHNOLOGY**: Cloudera, On-premise data warehouse, Amazon S3, Amazon Redshift/Redshift Spectrum, Talend Data Studio, Tableau

---

### (2020) IRIS - Employee Timekeeping System

![IRIS - Employee Timekeeping System](<img width="776" height="340" alt="image" src="https://github.com/user-attachments/assets/082372a6-4d4d-4faf-b33f-4cd3cf315f5d" />
)

**DESCRIPTION**: The project aims to streamline employee attendance management by implementing a facial recognition-based timekeeping system. Instead of relying on traditional ID cards or biometric fingerprint scanners, the solution automatically identifies employees as they enter or leave the office, accurately recording their time-in and time-out events while maintaining a centralized attendance database.

**HOW IT WORKS**: Cameras installed at the office entrance capture live video feeds of employees entering and exiting the premises. The captured faces are processed using a facial recognition model, which matches them against a registered employee database. Once a match is verified, the system automatically logs the corresponding time-in or time-out record. Attendance data is then stored in a centralized database, where it is used to generate reports, monitor employee attendance, calculate working hours, and provide dashboards for HR and management.

**TECHNOLOGY**: Python, OpenCV Face Recognition, TensorFlow, Django, PostgreSQL/MySQL, REST API, Tableau
