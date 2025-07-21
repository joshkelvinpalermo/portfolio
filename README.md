# Data Engineering Portfolio

Hi! My name is Josh, and I'm thrilled to share my growing professional portfolio with you. This repository contains a curated collection of projects completed through various data engineering and analytics stints, self-directed learning exercises, and company-initiated projects. Each project highlights key skills and techniques in the field.

## Company Projects

### Core Data Migration (2025)
<img width="507" height="560" alt="MDM" src="https://github.com/user-attachments/assets/d7e6b027-1bfa-44a5-8e80-49f43526f2a7" />
**DESCRIPTION**: The project aims to transition all master data processing workloads from a legacy environment, which relies on custom-built ETL pipelines for individual sub-domains, to a refreshed data mesh framework. This new framework is fully parameterized and driven entirely by JSON configurations that enables scalability and dynamic pipeline orchestration across several master data domains.

**HOW IT WORKS**:

**TECHNOLOGY**:

### CleverSense (2024)

![CleverSense](https://github.com/user-attachments/assets/bd7f5eea-f044-4d4f-b7a3-5a014eb51566)

**DESCRIPTION**: This project focuses on building and maintaining an end-to-end data pipeline to collect, process, and analyze sensors, machines, and factory data from various industrial machines. The system captures real-time data from these devices, dumps them in parquet format, and is processed for analytics. Using data engineering techniques like data aggregation, transformation, and time-series analysis via Azure Databricks, the project aims to monitor machine performance, product manufacturing, and improve operational efficiency.

**HOW IT WORKS**: Several machines from the many plants and factories of the company have sensors, PLCs, and devices that generates real-time data. These raw data in the form of parquet files are ingested and stored into Data Lake, then using Databricks, these are cleaned and processed. Curated data would then be loaded into Delta Lake and is projected on Microsoft Power BI for reporting.

**TECHNOLOGY**: Azure Data Lake, Azure Data Factory, Azure Databricks, Azure Synapse Analytics, Power BI

---

### Finance Group - Global Sourcing, International Supply Chain (2024)

![Finance Group](https://github.com/user-attachments/assets/a3b61c77-f5ac-4f47-99df-af9e620d2c42)

**DESCRIPTION**: The aim of the project was to streamline the data management and analysis processes for one of the financial legs of the company. It focused on gathering, cleaning, transforming, and storing large volumes of financial data to provide actionable insights for financial analysis, forecasting, and reporting. By building a robust data pipeline and integrating various data sources, the project ensures that decision-makers have access to real-time, accurate, and comprehensive financial data.

**HOW IT WORKS**: The raw data are being extracted from SAPS4/HANA using an application built on Azure App Service, then dumped on Data Lake. Using the JSON configuration files that we developed, these data are processed and transformed based on the rules, mappings, and transformations that are defined, including the join, primary, and surrogate keys. The purpose of these JSON files were so we can just dynamically apply several transformation methods using only one framework. Cleaned and structured data would then be stored on the Delta Lake and is loaded to Tableau as the serving layer.

**TECHNOLOGY**: SAPS4/4HANA, Azure Data Lake, Azure Data Factory, Azure Databricks, Azure Synapse Analytics, Power BI

## Personal Projects
### [Pseudo-Pokedex - VGG Net](https://github.com/joshkelvinpalermo/Pokedex)
Description: This project was built using the VGG Net convolutional neural network model and was trained on thousands of Pokemon images. The model predicts the name of the Pokemon based on the user's input image.
Technology: VGG Net, python, web scraping

