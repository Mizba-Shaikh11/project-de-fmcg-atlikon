# AtliQ Data Engineering Project

## Project Overview

This project implements an end-to-end data engineering pipeline for processing FMCG sales data and preparing it for analytics and reporting.

The pipeline uses **Databricks and PySpark** to ingest, clean, transform, and organize data using a **Medallion Architecture**. The processed data is stored using **Delta Lake** and structured into analytics-ready datasets.

## Tech Stack

* **Databricks**
* **PySpark**
* **Python**
* **SQL**
* **Apache Spark**
* **Delta Lake**
* **Medallion Architecture**
* **Git & GitHub**

## Architecture

The project follows a layered data processing approach:

```text
Raw Data
   │
   ▼
Bronze Layer
   │
   │  Data Ingestion
   ▼
Silver Layer
   │
   │  Cleaning & Transformation
   ▼
Gold Layer
   │
   │  Business-ready Data
   ▼
Analytics & Reporting
```

### Bronze Layer

The Bronze layer contains the raw ingested data with minimal transformation. It preserves the source data for further processing.

### Silver Layer

The Silver layer contains cleaned and transformed datasets. Data quality, standardization, filtering, and transformation operations are performed at this stage.

### Gold Layer

The Gold layer contains structured, business-ready datasets designed for analytical use cases and reporting.

## Data Engineering Workflow

### 1. Data Ingestion

Raw FMCG datasets are loaded into the Databricks environment for processing.

### 2. Data Cleaning

The raw data is cleaned and standardized using PySpark transformations, including:

* Handling missing values
* Removing or handling inconsistent records
* Data type conversion
* Column standardization
* Data validation

### 3. Dimension Data Processing

Dimension datasets are processed and transformed to create clean, structured dimensional data for downstream analytics.

### 4. Fact Data Processing

Fact datasets are processed using PySpark and prepared for analytical workloads.

### 5. Delta Lake

Processed datasets are stored using Delta Lake to provide a reliable storage layer for the data pipeline.

### 6. Analytics-Ready Data

The final processed datasets are organized for downstream analytics and reporting.

## Project Structure

```text
AtliQ-Data-Engineering-Project/
│
├── README.md
│
├── code/
│   ├── 1_Setup/
│   ├── 2_Dimenssion_Data_Processing/
│   └── 3_fact_data_processing/
│
├── resources/
│   └── ...
│
└── data/
    └── ...
```

## Key Data Engineering Concepts

* ETL / ELT
* Data ingestion
* Data cleaning and transformation
* PySpark DataFrames
* Apache Spark
* Medallion Architecture
* Delta Lake
* Dimension and fact data processing
* Data quality and validation
* Analytics-ready data preparation

## Project Outcome

The project demonstrates an end-to-end data engineering workflow that transforms raw FMCG data into structured, analytics-ready datasets.

It provides practical experience in building data pipelines using **Databricks, PySpark, Delta Lake, and Medallion Architecture**.
