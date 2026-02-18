# Architecture Overview

This document describes the technical architecture of the **Intelligent Data Monitoring Automation** built with n8n.

The solution is designed to be **modular, reliable, and easy to maintain**, following a clear data flow from ingestion to alert delivery.

---

## Data Sources

The automation consumes **structured data** from the following possible sources:

- Google Sheets (operational metrics)
- CSV / JSON files
- Databases (via SQL queries)
- APIs (when applicable)

All data used for documentation and testing purposes is **fictitious and anonymized**.

---

## Data Processing Flow

The workflow follows these main steps:

1. **Data Ingestion**  
   Data is collected from the configured source and validated to ensure required fields are present.

2. **Normalization & Validation**  
   - Data types are validated  
   - Missing or invalid values are handled  
   - Metrics are standardized for processing  

3. **Metric Evaluation**  
   Key indicators are calculated, such as:
   - Current value
   - Previous value
   - Percentage variation

4. **Business Rule Evaluation**  
   Predefined business rules are applied to detect anomalies and abnormal behavior.

5. **Severity Classification**  
   Each metric is classified as:
   - Normal  
   - Warning  
   - Critical  

---

## Alerts

When a rule is triggered, the workflow generates an automated alert containing:

- Metric name
- Detected variation
- Severity level
- Timestamp
- Recommended action

Alerts are designed to be **clear, concise, and actionable**.

---

## Integrations

The solution supports integration with:

- Communication tools via Webhooks
- Business Intelligence tools (Power BI, Looker Studio)
- Other automation workflows

The architecture allows easy extension without impacting existing logic.

---

## Design Principles

- Modular workflow design  
- Clear separation between data ingestion, processing, and alerting  
- Easy maintenance and scalability  
- Business-oriented logic  

---

## Summary

This architecture ensures reliable monitoring of operational data while providing timely and actionable alerts to support decision-making.
