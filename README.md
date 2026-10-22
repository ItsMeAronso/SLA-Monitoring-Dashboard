# SLA-Monitoring-Dashboard
Automated SLA monitoring data pipeline and dashboard for shipping providers, built with Python and Power BI.

# Vendor Performance & SLA Dashboard

## Overview
This dashboard was developed to enable the team to monitor and investigate vendor (courier) performance over the past week. The analysis provides a clear breakdown of operations by country, specific vendor, and SLA compliance.

Target Audience & Use Case
This dashboard is not intended for high-level organizational vendor evaluation or procurement purposes. Rather, it is an operational, day-to-day management tool designed for the internal team. It provides visibility into the ongoing status with various couriers, guides daily interactions, and helps quickly identify communication gaps or operational bottlenecks over specific time periods.

## Business Context: SLA Requirements
SLA terms vary per shipment. While the standard requirement is Next Business Day (NBD) delivery, certain shipments have stricter constraints, such as exact day/hour deliveries or short-window same-day drop-offs. 

## Data Pipeline & Architecture
In the real-world workflow, data is extracted weekly, cleaned, merged, and updated in a cloud repository. To replicate this environment for the portfolio without exposing sensitive information, I built an automated data pipeline:
* **Synthetic Data Generation:** Created three separate datasets (Orders, Customers, and Addresses) that mimic the exact structure of the original data.
* **Data Processing:** Developed a Python script to clean and merge these separate tables into a single unified master table for analysis.

** Data Privacy Notice:** All data included in this repository is 100% synthetic and generated exclusively for demonstration purposes to ensure absolute data privacy and security.
