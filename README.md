# Real-Time-Streaming-End-to-End-Project
# 🚴‍♂️ Real-Time Bike Monitoring Dashboard using Microsoft Fabric

This project demonstrates an end-to-end **Real-Time Intelligence solution** built using **Microsoft Fabric**, showcasing real-time data ingestion, transformation, visualization, and alerting for a bike-sharing dataset.

---

## 📌 Project Overview

We’ve implemented a real-time analytics pipeline that:
- Ingests streaming data using **Eventstream**
- Stores raw data in the **Eventhouse (Bronze Layer)**
- Transforms and enriches data into the **Silver Layer**
- Aggregates data in the **Gold Layer** using **Materialized Views**
- Visualizes insights in a **Real-Time Dashboard**
- Sends alerts via **Data Activator** based on business rules

---

## 🔧 Technologies Used

- Microsoft Fabric  
- Eventstream  
- KQL Database (Eventhouse)  
- Update Policy  
- Materialized Views  
- Real-Time Dashboard  
- Data Activator  
- Power BI (optional advanced visuals)

---

## 🔄 Architecture

```plaintext
Live Bike Data → Eventstream → Eventhouse (Bronze)
                             ↓
           Function + Update Policy → Silver Layer
                             ↓
           Materialized View → Gold Layer
                             ↓
         Real-Time Dashboard + Data Activator
