#  Retail Data Analysis using PySpark in Azure Databricks

This project demonstrates a retail data analysis and transformation pipeline** built with PySpark in the Azure Databricks environment.  
It focuses on data cleaning, date-time processing, joins, and saving transformed outputs to *Parquet format* for downstream analytics.

---

##  Project Overview

The main goal of this project is to prepare and transform raw retail data for analytical use within Azure Databricks.  
It leverages **PySpark** for distributed data processing and integrates with **Unity Catalog** for data governance and secure storage.

---

##  Data Cleaning and Transformation Steps

1. **Load Data**
   - Data is ingested from a source registered in **Unity Catalog**.
   - The data is loaded into a PySpark DataFrame for processing.

2. **Data Cleaning**
   - Remove **null values** and handle missing data appropriately.
   - Perform basic data type validation and schema consistency checks.

3. **Date and Time Transformation**
   - Extract the **year** component from transaction timestamps.
   - Create derived columns for time-based analytics
     
4. **Join Operations**
   - Perform **inner** between datasets.
   - Ensure join keys are cleaned and consistent before merging.

5. **Data Validation**
   - Validate row counts and schema after each transformation step.
   - Log transformation steps for reproducibility.

6. **Save Transformed Data**
   - Write the cleaned and transformed dataset into **Parquet format**.
   - Store the output securely in a **Unity Catalog volume** for downstream BI or reporting use cases.

---

##  Technologies Used

| Component | Description |
|------------|-------------|
| **Azure Databricks** | Cloud-based environment for data engineering and analytics |
| **PySpark** | Distributed data processing framework used for ETL operations |
| **Unity Catalog** | Centralized governance for data access and lineage |
| **Parquet** | Columnar storage format optimized for performance and compression |
