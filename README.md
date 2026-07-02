
# 🎓 Student Success Intelligence Platform (SSIP)

> **Enterprise Learning Analytics Built on the Databricks Lakehouse**

<p align="center">
  <img src="images/github_banner.png" width="100%">
</p>

<p align="center">

![Databricks](https://img.shields.io/badge/Databricks-EF3E42?style=for-the-badge&logo=databricks&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Delta Lake](https://img.shields.io/badge/Delta%20Lake-0A84FF?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Spark SQL](https://img.shields.io/badge/Spark_SQL-336791?style=for-the-badge)
![Lakeview](https://img.shields.io/badge/Lakeview-Dashboard-6C63FF?style=for-the-badge)

</p>

---

# 📑 Table of Contents

- Overview
- Business Problem
- Platform Overview
- Enterprise Architecture
- Project Highlights
- Project Metrics
- Technology Stack
- Data Model
- Repository Structure
- Enterprise Semantic Layer
- Dashboard Showcase
- Business Impact
- Engineering Decisions
- Future Roadmap
- Getting Started
- Author

---

# 📖 Overview

The **Student Success Intelligence Platform (SSIP)** is an enterprise learning analytics platform built on the Databricks Lakehouse. It centralizes student information, enrollments, attendance, Blackboard LMS activity, and academic performance into a unified analytics environment that supports executive reporting, student success initiatives, and academic planning.

Designed using a Medallion (Bronze, Silver, Gold) architecture, the platform demonstrates enterprise-grade data engineering, analytics engineering, semantic modeling, and business intelligence.

---

# 🎯 Business Problem

Universities generate millions of academic and learning management records every semester. These datasets are often distributed across disconnected systems, making it difficult to identify students who need support, monitor institutional performance, and make timely decisions.

The Student Success Intelligence Platform provides a unified analytics solution that transforms operational data into actionable intelligence for executives, academic advisors, and department leaders.

---

# 💡 Platform Overview

The platform ingests academic and Blackboard LMS data into a Databricks Lakehouse, applies scalable ETL transformations, engineers student success features, and exposes reusable Gold semantic views powering interactive Lakeview dashboards.

It supports:

- Executive reporting
- Student success monitoring
- Academic intervention prioritization
- Department performance benchmarking
- Course-level analytics

---

# 🏗 Enterprise Architecture

![Architecture](architecture/lakehouse_architecture.png)

The platform follows a Medallion Architecture:

- **Bronze Layer** – Raw operational data
- **Silver Layer** – Cleaned, standardized, and integrated datasets
- **Gold Layer** – Business-ready semantic views and KPIs
- **Lakeview Dashboards** – Executive analytics and decision support

---

# 🚀 Project Highlights

- Built an enterprise learning analytics platform on Databricks Lakehouse.
- Processed **1.3M+ student activity records** and **7.5M Blackboard LMS events**.
- Developed **13 reusable Gold semantic views**.
- Built **3 executive Lakeview dashboards**.
- Implemented a rule-based student intervention engine.
- Applied dimensional modeling, feature engineering, and semantic analytics.

---

# 📊 Project Metrics

| Metric | Value |
|---------|------:|
| Students | 8,500 |
| Active Enrollments | 147,442 |
| Student Activity Records | 1,316,173 |
| Blackboard LMS Events | ~7.5 Million |
| Departments | 9 |
| Courses | 19 |
| Gold Semantic Views | 13+ |
| Interactive Dashboards | 3 |

---

# 🛠 Technology Stack

| Category | Technologies |
|----------|--------------|
| Platform | Databricks Lakehouse |
| Storage | Delta Lake |
| Processing | Apache Spark, Spark SQL |
| Programming | Python, SQL |
| Analytics | Databricks SQL |
| Visualization | Lakeview Dashboards |
| Architecture | Medallion Architecture |
| Version Control | Git, GitHub |

---

# 🏛 Data Model

Core entities include:

- Students
- Enrollments
- Courses
- Departments
- Semester Calendar
- Blackboard LMS Events
- Student Daily Activity
- Student Success Features
- Course Performance Summary
- Department Performance Summary

---

# 📂 Repository Structure

```text
student-success-intelligence-platform/
├── architecture/
├── dashboards/
├── docs/
├── images/
├── notebooks/
├── sample_data/
├── screenshots/
├── sql/
├── README.md
└── LICENSE
```

---

# 📈 Enterprise Semantic Layer

Executive Analytics

- vw_executive_kpis
- vw_daily_lms_trend
- vw_department_performance
- vw_course_risk_ranking
- vw_risk_distribution

Student Success

- vw_behavior_profile_performance
- vw_student_level_performance
- vw_engagement_correlation
- vw_intervention_priority
- vw_priority_outreach_queue

Academic Analytics

- vw_department_summary
- vw_course_summary
- vw_course_enrollment

---

# 📊 Dashboard Showcase

## Executive Overview

Audience: University Leadership

Highlights:

- Executive KPIs
- Academic Risk Distribution
- LMS Activity Trends
- Department Performance
- Course Risk Ranking

![Executive Dashboard](screenshots/executive_overview.png)

---

## Student Success & Retention

Audience: Academic Advisors

Highlights:

- Student Engagement
- Behavior Profiles
- Risk Analysis
- Priority Outreach Queue
- Intervention Insights

![Student Success](screenshots/student_success.png)

---

## Course & Department Analytics

Audience: Department Chairs

Highlights:

- Department Performance
- Course Enrollment
- Department Engagement
- Course Risk Ranking
- Course Performance Summary

![Course Analytics](screenshots/course_department.png)

---

# 🌟 Business Impact

The Student Success Intelligence Platform demonstrates how a modern Lakehouse architecture can improve institutional analytics by:

- Identifying academically at-risk students earlier.
- Supporting proactive academic interventions.
- Delivering executive visibility into institutional performance.
- Benchmarking departments and courses.
- Providing a reusable semantic analytics layer for future AI initiatives.

---

# ⚙️ Engineering Decisions

- Medallion Architecture for scalable data processing.
- Delta Lake for reliable ACID data storage.
- Gold semantic views to separate business logic from reporting.
- Lakeview dashboards tailored to executive, advisor, and department stakeholder needs.
- Feature engineering to derive engagement scores and intervention priorities.

---

# 🚀 Future Roadmap

- Machine learning-based student success prediction.
- AI-powered academic advisor assistant.
- Generative AI intervention recommendations.
- Real-time Blackboard event streaming.
- Power BI and Tableau integrations.
- AWS deployment and CI/CD automation.

---

# ▶️ Getting Started

```bash
git clone https://github.com/OmkarK23/learning-analytics-lakehouse-platform.git
```

Execution order:

1. Load sample academic datasets
2. Create Bronze tables
3. Build Silver transformations
4. Generate Gold semantic views
5. Execute SQL analytics
6. Build Lakeview dashboards

---

# 👤 Author

**Omkar Kalekar**

MS in Information Systems  
University of Maryland, Baltimore County

- GitHub: https://github.com/OmkarK23
- LinkedIn: https://www.linkedin.com/in/omkar-kalekar/
- Portfolio: https://omkark23.github.io/portfolio-website/

---

## ⭐ If you found this project useful, consider giving it a star.
