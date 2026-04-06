# Azure End-to-End ETL Pipeline – Capstone Project

## Project Overview

This project demonstrates the design and implementation of a simple end-to-end ETL (Extract, Transform, Load) pipeline using Microsoft Azure services.

The pipeline ingests a raw sales dataset, processes it using Azure Data Factory, stores the curated output in Azure Blob Storage, and visualizes the results in Power BI.

The objective of this project is to demonstrate foundational data engineering skills including cloud storage management, data orchestration, and data visualization.

---

## Technologies Used

- Microsoft Azure
- Azure Blob Storage
- Azure Data Factory
- Power BI Desktop
- CSV dataset

---

## Architecture Overview

The ETL workflow follows this structure:

Raw Data → Azure Blob Storage → Azure Data Factory → Curated Storage → Power BI Dashboard

Steps:

1. Raw data is uploaded to Azure Blob Storage (raw container)
2. Azure Data Factory orchestrates the pipeline
3. Data is processed and copied into a curated dataset
4. Curated data is used for analytics
5. Power BI creates visual insights from the dataset

---

## Dataset

The dataset used in this project is a retail sales dataset stored in CSV format.

It contains transactional sales data including:

- Product
- Category
- Quantity
- Price
- Region
- Order Date

This dataset enables analysis of sales performance across products, categories, and geographic regions.

---

## Project Steps

### 1. Azure Environment Setup

- Created a Resource Group
- Created an Azure Storage Account
- Created two Blob containers:
  - raw
  - curated

---

### 2. Data Upload

The dataset `sales_raw.csv` was uploaded to the **raw container** in Azure Blob Storage.

---

### 3. Azure Data Factory Pipeline

A pipeline was created in Azure Data Factory to copy the dataset from the raw container to the curated container.

Pipeline components include:

- Linked Service connection to Azure Storage
- Source dataset (raw)
- Sink dataset (curated)
- Copy Data Activity

---

### 4. Pipeline Execution

The pipeline was executed and verified through the **Azure Data Factory Monitor panel**.

After execution, the curated dataset was successfully written to the curated container.

---

### 5. Data Visualization

The curated dataset was imported into **Power BI Desktop** to build a dashboard showing:

- Total revenue
- Sales by region
- Sales by product
- Sales by category
- Sales trend over time

---

## Project Structure

```
Azure-ETL-Capstone
│
├── README.md
├── sales_raw.csv
├── screenshots/
│   ├── data_factory_pipeline.png
│   ├── azure_storage_raw.png
│   ├── curated_output.png
│   ├── pipeline_monitor.png
│   └── powerbi_dashboard.png
│
└── powerbi/
    └── sales_dashboard.pbix
```

This structure organizes the project files including the dataset, dashboard, and screenshots of the ETL pipeline.

---

## Power BI Dashboard

The dashboard provides insights into:

- Total revenue
- Regional sales distribution
- Product performance
- Category breakdown
- Sales trends over time

This allows users to quickly understand key sales metrics and patterns.

---

## Key Learning Outcomes

This project demonstrates:

- Cloud storage management using Azure Blob Storage
- Data pipeline orchestration using Azure Data Factory
- Basic ETL workflow implementation
- Data visualization using Power BI
- End-to-end cloud data engineering workflow

---

## Cleanup Checklist

To avoid unnecessary Azure charges after completing the project, the following resources should be removed:

- [ ] Stop any running Azure Data Factory pipelines
- [ ] Delete the Azure Data Factory instance
- [ ] Delete the Azure Storage Account
- [ ] Remove Blob containers (raw and curated)
- [ ] Delete the Resource Group created for this project

The easiest method is to delete the **entire Resource Group**, which removes all associated resources at once.

---

## Author

Newton Mirang'a  
Data Science Capstone Project