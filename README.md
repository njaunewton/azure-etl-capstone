# Azure End-to-End ETL Capstone Project

## Overview

This project demonstrates the design and implementation of a simple end-to-end ETL (Extract, Transform, Load) data pipeline using Microsoft Azure cloud services.

The pipeline extracts a raw sales dataset, processes it using Azure Data Factory, stores the cleaned data in Azure Blob Storage, and visualizes the results using Power BI.

This project showcases how cloud tools can be integrated to create a scalable and automated data workflow.

---

## Technologies Used

- Microsoft Azure
- Azure Blob Storage
- Azure Data Factory
- Power BI Desktop
- Git & GitHub

---

## Project Architecture

1. Raw dataset uploaded to Azure Blob Storage (raw container)
2. Azure Data Factory pipeline extracts and processes the data
3. Transformed dataset stored in the curated container
4. Power BI connects to curated dataset
5. Dashboard created to analyze sales performance

---

## Project Structure

```
azure-etl-capstone
│
├── README.md
│
├── data
│   ├── sales_raw.csv
│   └── sales_curated.csv
│
├── powerbi
│   └── etl_sales_dashboard.pbix
│
├── report
│   ├── Newton_Capstone_Azure End-to-End ETL.docx
│   └── Newton_Capstone_Azure End-to-End ETL.pdf
│
└── screenshots
    ├── azure_storage_raw.png
    ├── curated_output.png
    ├── data_factory_pipeline.png
    ├── pipeline_monitor.png
    └── powerbi_dashboard.png
```

---

## Power BI Dashboard

Example visualization generated from the curated dataset.

![Power BI Dashboard](screenshots/powerbi_dashboard.png)

---

## Pipeline Execution

Azure Data Factory pipeline execution example.

![ADF Pipeline](screenshots/data_factory_pipeline.png)

---

## Cleanup Checklist

After completing the project, the following Azure resources should be cleaned up to avoid unnecessary charges:

- Delete the Azure Resource Group
- Remove Azure Storage Account
- Delete Azure Data Factory instance
- Remove any associated datasets and pipelines

---

## Author

Blessed Newton  
NACIT Data Science Program