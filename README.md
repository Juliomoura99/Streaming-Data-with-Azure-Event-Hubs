# Streaming Data with Azure Event Hubs

This project demonstrates an end-to-end solution for **real-time data streaming and analytics** using **Azure Event Hubs**, **Azure Databricks**, **Unity Catalog**, and **Power BI**.

The main goal of this project is to build a streaming data pipeline capable of ingesting events in real time, processing them with Apache Spark Structured Streaming, organizing the data using the **Medallion Architecture**, and making the curated data available for analytical consumption and visualization.

---

## 📌 Project Overview

Modern data platforms often need to process data continuously instead of relying only on batch pipelines. This project simulates a real-time streaming scenario where event data is ingested through **Azure Event Hubs**, processed in **Azure Databricks**, and prepared for visualization in **Power BI**.

The pipeline follows the **Bronze, Silver, and Gold** layer approach:

```text
Event Producer
      ↓
Azure Event Hubs
      ↓
Azure Databricks Structured Streaming
      ↓
Bronze Layer
      ↓
Silver Layer
      ↓
Gold Layer
      ↓
Power BI
