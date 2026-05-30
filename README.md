# ⚙️ Intelligent Data Monitoring Automation (n8n)

![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Webhooks](https://img.shields.io/badge/Webhooks-FF6B35?style=for-the-badge)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Automation](https://img.shields.io/badge/Automation-4CAF50?style=for-the-badge)
![Data Monitoring](https://img.shields.io/badge/Data_Monitoring-2196F3?style=for-the-badge)
![Alert System](https://img.shields.io/badge/Alert_System-D32F2F?style=for-the-badge)

## Overview

This project is an **intelligent data monitoring and alert automation** built using **n8n**, designed to automatically analyze operational data and notify teams when anomalies or critical situations are detected.

The solution was **developed and presented during my internship**, where it received **excellent feedback** for its clarity, usefulness, and real business impact.

---

## Business Problem

Operational and business teams often face challenges such as:

- Manual monitoring of large datasets  
- Delayed identification of data drops or anomalies  
- Lack of automated alerts  
- High dependency on manual checks  

These issues increase operational risk and slow down decision-making.

---

## Solution

This automation acts as a **virtual data analyst**, continuously monitoring key metrics and generating alerts when predefined conditions are met.

The workflow:

1. Ingests structured data (tables / spreadsheets / JSON)
2. Processes key indicators such as:
   - Volume
   - Percentage variation
   - Threshold breaches
3. Applies business rules to classify severity
4. Automatically sends alerts to communication channels
5. Supports integration with dashboards and BI tools

---

## Architecture

**Main components:**

- n8n workflows  
- Data source (structured tables / spreadsheets / APIs)  
- Business rules and validation logic  
- Alert delivery via webhook  
- Optional BI integration (Power BI / Looker Studio)

---

## Technologies Used

- n8n  
- SQL  
- Python (for data preparation, when applicable)  
- Webhooks  
- Git & GitHub  

---

## Key Features

- Automated daily monitoring  
- Detection of abnormal variations  
- Severity classification (low / medium / high)  
- Real-time alerts  
- Modular and scalable workflow design  
- Easy adaptation to different datasets  

---

## Internship Context

This project was developed as part of my **internship**, where I:

- Designed the full automation logic  
- Defined monitoring rules with business context  
- Implemented the workflow in n8n  
- Presented the solution to stakeholders  
- Received strong positive feedback for clarity and effectiveness  

---

## Example Alert

```text
🚨 CRITICAL ALERT

Metric: Data Volume Drop
Variation: -32%
Impact: High

Recommended Action:
Investigate upstream data pipeline or source availability.
```
--- 
*Created by Brenda Espinosa*
