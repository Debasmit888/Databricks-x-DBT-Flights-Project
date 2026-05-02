Project Overview: End-to-End Flights Data Pipeline
This project demonstrates a complete Medallion Architecture (Bronze, Silver, Gold) pipeline built on Databricks. It processes raw flight data into refined tables optimized for analytics and business intelligence.

Technical Architecture
The pipeline follows the Medallion Design Pattern to ensure data quality and reliability:

Bronze Layer (BronzeLayer.python): Handles initial ingestion of raw flight data from source to Delta tables.

Silver Layer (SilverNotebook.python): Performs data cleaning, filtering, and schema enforcement.

Gold Layer (GOLD_DIMS.python, GOLD_FACTS.python): Creates optimized Dimension and Fact tables for analytics, such as airport details and flight performance metrics.


Key Features
Delta Live Tables (DLT): Utilizes the DLT/ folder components to define declarative ETL pipelines with built-in data quality monitoring.

Parameterization: Uses SrcParameters.python to maintain a flexible, environment-agnostic configuration.

PySpark & SQL: Leverages both PySpark for complex transformations and SQL for final data modeling.
