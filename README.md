📌 Project Overview

->This project demonstrates the design and implementation of a SQL-based Data Warehouse using the Medallion Architecture (Bronze, Silver, Gold layers).
->The goal is to transform raw operational data into a clean, analytical, business-ready star schema for reporting and dashboarding.

->The project uses sample / random datasets to simulate real-world business scenarios.

🏗️ Architecture Overview
->Bronze Layer (Raw Data)

->Stores raw ingested data from multiple source systems (CRM & ERP).

->Data is loaded as-is with minimal transformations.

->Silver Layer (Cleaned Data)

->Cleans and standardizes Bronze data.

Handles:

->Null values

->Data type corrections

->Data consistency

->Prepares data for analytical modeling.

->Gold Layer (Business Layer)

->Implements a Star Schema using SQL Views.

->Provides dimension and fact views for analytics and BI tools.

No data duplication — data is queried dynamically from Silver layer.
