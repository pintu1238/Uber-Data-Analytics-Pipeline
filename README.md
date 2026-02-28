# Uber Data Analytics Platform | Modern Data Engineering on GCP

## Overview

This project demonstrates an end-to-end data engineering pipeline built on Google Cloud Platform to analyze Uber trip data.

The solution covers the complete lifecycle — from raw data ingestion and transformation to dimensional modeling, analytical querying, and dashboard creation.

---

## Architecture

Raw Data (Uber Trip Records)  
→ Google Cloud Storage  
→ Mage ETL (Compute Engine VM)  
→ BigQuery (Analytics Layer)  
→ Looker Studio (Dashboard & Reporting)

---

## Tech Stack

### Programming
- Python

### Google Cloud Platform
- Google Cloud Storage (Raw Data Layer)
- Compute Engine (Mage ETL Runtime)
- BigQuery (Data Warehouse & Analytics)
- Looker Studio (Business Intelligence)

### ETL Orchestration
- Mage (Modern Data Pipeline Tool)

---

## Dataset

New York TLC Trip Record Data

The dataset includes:
- Pickup and drop-off timestamps  
- Pickup and drop-off locations (latitude & longitude)  
- Trip distance  
- Passenger count  
- Fare amount and itemized charges  
- Rate codes and payment types  

---

## Data Modeling

A dimensional star schema was implemented.

### Fact Table
- Trip-level transactional data

### Dimension Tables
- Datetime
- Passenger Count
- Trip Distance
- Rate Code
- Payment Type
- Pickup Location
- Drop Location

<img src="data_model.jpeg">

---

## Key Features

- Built a cloud-native ETL pipeline using Mage on Compute Engine
- Implemented star schema dimensional modeling for analytical efficiency
- Performed data cleansing and transformation using Python
- Loaded curated datasets into BigQuery for scalable querying
- Designed interactive dashboards in Looker Studio to visualize KPIs such as:
  - Total Revenue
  - Average Fare
  - Trip Distance
  - Geospatial Pickup & Drop Trends

---

## Outcome

This project demonstrates:
- End-to-end data pipeline design on GCP
- Practical dimensional modeling
- Cloud-based analytics using BigQuery
- Business-ready dashboard creation
