# Business Rules Documentation

## Purpose

This document describes the business rules applied in the automated monitoring workflow.
These rules are designed to detect anomalies, significant variations, and operational risks in a reliable and transparent way.

All rules are implemented and executed automatically within the n8n workflow.

---

## Monitored Metrics

The system evaluates the following types of metrics:

- Volume of records processed
- Percentage change compared to previous periods
- Threshold-based limits defined by business requirements

These metrics can be extended depending on future monitoring needs.

---

## Rule 1: Volume Drop Detection

### Description
Detects sudden drops in data volume compared to an expected baseline.

### Logic
- Calculate the current volume
- Compare it with a predefined threshold
- Trigger an alert if the current value falls below the acceptable limit

### Example
```text
If current_volume < minimum_expected_volume → trigger alert
