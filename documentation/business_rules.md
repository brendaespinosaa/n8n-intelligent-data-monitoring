# Business Rules Documentation

This document defines the business rules used to detect anomalies and trigger alerts in the monitoring automation.

---

## Monitored Metrics

Examples of monitored metrics include:

- Order volume
- Active users
- Transaction count
- Any numerical operational KPI

The rules are generic and can be adapted to different datasets.

---

## Percentage Variation Calculation

The percentage variation is calculated using the following logic:

Variation (%) = ((Current Value - Previous Value) / Previous Value) * 100

---

## Alert Thresholds

The system classifies alerts based on the percentage variation:

| Severity  | Variation Range        |
|----------|------------------------|
| Normal   | ≥ -10%                 |
| Warning  | < -10% and ≥ -25%      |
| Critical | < -25%                 |

---

## Alert Conditions

An alert is triggered when:

- The variation exceeds the defined threshold
- The metric status is classified as **Warning** or **Critical**

Normal variations are logged but do not generate alerts.

---

## Alert Content

Each alert includes:

- Metric name  
- Current value  
- Previous value  
- Percentage variation  
- Severity level  
- Suggested action  

---

## Example Rule

```text
IF percentage_variation < -25%
THEN severity = "Critical"
AND trigger alert
