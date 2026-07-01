# Learning Analytics Lakehouse Platform Architecture

## Overview

The Learning Analytics Lakehouse Platform follows the Medallion (Bronze, Silver, Gold) architecture on Databricks. Raw university data from multiple operational systems is ingested into Bronze tables, transformed into standardized Silver tables, and curated into Gold semantic views that power executive dashboards and analytics.

---

## Architecture Diagram

```mermaid
flowchart TB

subgraph DataSources["📥 Data Sources"]
A1["Students"]
A2["Enrollments"]
A3["Courses"]
A4["Departments"]
A5["Semester Calendar"]
A6["Blackboard LMS Events"]
A7["Student Daily Activity"]
end

subgraph Bronze["🥉 Bronze Layer (Raw Delta Tables)"]
B1["Raw Student Data"]
B2["Raw Enrollment Data"]
B3["Raw Blackboard Events"]
B4["Raw Daily Activity"]
end

subgraph Silver["🥈 Silver Layer (Cleaned &Standardized)"]
S1["Students"]
S2["Enrollments"]
S3["Courses"]
S4["Departments"]
S5["Daily Activity"]
S6["Behavior Profiles"]
end

subgraph Gold["🥇 Gold Semantic Layer"]
G1["Semester KPIs"]
G2["Course Performance Summary"]
G3["Department Performance Summary"]
G4["Student Success Features"]
G5["Executive KPI Views"]
G6["Risk Distribution Views"]
G7["Intervention Priority Views"]
end

subgraph Dashboards["📊 Databricks Lakeview Dashboards"]
D1["Executive Overview"]
D2["Student Success & Retention"]
D3["Course & Department Analytics"]
end

A1 --> B1
A2 --> B2
A3 --> B2
A4 --> B2
A5 --> B2
A6 --> B3
A7 --> B4

B1 --> S1
B2 --> S2
B2 --> S3
B2 --> S4
B3 --> S5
B4 --> S6

S1 --> G4
S2 --> G2
S3 --> G2
S4 --> G3
S5 --> G4
S6 --> G4

G4 --> G5
G4 --> G6
G4 --> G7

G2 --> D3
G3 --> D3
G5 --> D1
G6 --> D1
G7 --> D2
G4 --> D2
```

---

## Medallion Architecture

### Bronze Layer
Stores raw synthetic university datasets exactly as generated with minimal transformation.

### Silver Layer
Applies cleansing, normalization, joins, and feature engineering to create standardized datasets for analytics.

### Gold Layer
Contains business-ready semantic views, aggregated metrics, KPIs, and intervention models that power dashboards.

---

## Dashboards Powered

### Executive Overview
- Executive KPIs
- Risk Distribution
- LMS Trends
- Department Performance
- Course Risk Ranking

### Student Success & Retention
- Student Engagement
- Behavior Profiles
- Risk Analysis
- Priority Outreach Queue

### Course & Department Analytics
- Department Performance
- Course Enrollment
- Course Risk
- Academic Performance

---

## Business Value

This architecture enables universities to:

- Centralize fragmented academic data
- Monitor student engagement
- Detect at-risk students early
- Support executive decision-making
- Improve institutional performance through data-driven interventions