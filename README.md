# Hi, I'm Aadityaa Dava

**Software Development Engineer (new grad)** | M.P.S. in Data Science, UMBC (graduating Dec 2026) | Baltimore, Maryland

Backend systems, data pipelines and cloud. Looking for full-time SDE roles starting January 2027.

---

## About Me

I build backend services and data pipelines, and I care about the parts that break in production: consistency across services, idempotency, failure handling and tests that can actually fail. I have shipped data processing and reporting systems at LTIMindtree and for a T-Mobile client through Valarcorp, and I build side projects to practice distributed-systems ideas end to end.

---

## Experience

**Software Development Engineer, Valarcorp (T-Mobile client)**, May 2026 to Aug 2026
Built backend profiling, transformation and validation processes in Python, PySpark and SQL over 1M+ records from multiple upstream systems, catching mismatched totals, bad records and late data before they reached executive reports.

**Software Development Engineer, LTIMindtree**, Mar 2024 to Dec 2024
Worked on client data and reporting systems: tuned SQL and ETL transformations (20% faster), automated a recurring reporting process, fixed a pipeline broken by an upstream schema change, and shipped through peer-reviewed pull requests.

**Graduate Assistant, UMBC**, Jan 2026 to May 2026
Supported 150+ students in Probability and Statistics for Data Science through labs, recitations and office hours.

---

## Featured Projects

### Order Platform: event-driven order processing

**Java 21 • Spring Boot • Kafka • PostgreSQL • Redis • Docker • Testcontainers • k6**

* Four services (order, inventory, payment, notification) keep data consistent without distributed transactions, using choreographed sagas with compensating events, a transactional outbox and idempotent consumers.
* Load-tested with k6 and fixed a consumer-thread bottleneck: sustainable throughput rose from about 22 to 85 orders/s (3.8x) on one laptop.
* Crashed services mid-saga to verify recovery: 601 of 601 orders confirmed after a `kill -9` under load.
* 40 test classes, an 80% coverage gate in GitHub Actions, and Prometheus, Grafana and OpenTelemetry observability.

[Repository](https://github.com/aadityaa-dava/order-platform)

---

### Multi-Tenant Invoicing API

**TypeScript • NestJS • PostgreSQL • Prisma • Redis • BullMQ**

* Tenant isolation with forced PostgreSQL row-level security and per-transaction tenant context.
* argon2id authentication with refresh-token rotation and reuse detection, plus role-based access control across four roles.
* Gapless invoice numbering, integer-cent money arithmetic, and idempotent background jobs (email, recurring invoices, overdue sweep).
* 200+ end-to-end tests against real PostgreSQL and Redis. Work in progress: Stripe, web frontend and deployment are planned.

[Repository](https://github.com/aadityaa-dava/invoicing-saas)

---

### Fraud Detection MLOps Pipeline

**Python • FastAPI • LightGBM • MLflow • DVC • Docker • GitHub Actions**

* Reproducible pipeline on the IEEE-CIS dataset with DVC data versioning, pandera validation and an MLflow model registry.
* 0.549 PR-AUC on a time-based test split (0.035 for random guessing).
* FastAPI service shipped as a Docker image through GitHub Actions CI/CD to a live Render deployment, with Evidently drift monitoring.

[Repository](https://github.com/aadityaa-dava/mlops-tabular-pipeline)

---

### RedLightWatch: edge red-light violation detector

**Python • YOLOv8 • ByteTrack • TensorRT • NVIDIA Jetson Orin Nano • Streamlit**

* Detects and tracks vehicles, reads the traffic-light colour and flags stop-line crossings on red, running a TensorRT FP16 engine at 8 to 13 FPS on the Jetson.
* Matched hand-labelled counts on all 9 test clips. Thresholds were tuned on those same clips, so real-world accuracy will be lower.

[Repository](https://github.com/aadityaa-dava/red-light-watch)

---

### Banking Analytics Engineering Platform

**PySpark • PostgreSQL • dbt • Airflow • Docker • Tableau**

* End-to-end pipeline on a synthetic dataset of 500K transactions, 50K customers and 20K loans: PySpark ETL, PostgreSQL star schema, dbt staging models and analytics marts.
* Five-stage Airflow DAG in Docker with row count, null and integrity checks, feeding Tableau executive dashboards.

[Repository](https://github.com/aadityaa-dava/banking-analytics-engineering-platform)

---

### More data work

* **[Healthcare Analytics Data Warehouse](https://github.com/aadityaa-dava/healthcare-analytics-data-warehouse):** Python ETL and a PostgreSQL star schema over Medicare provider utilization data, with Power BI dashboards.
* **[Healthcare Claims Fraud Detection](https://github.com/aadityaa-dava/healthcare-claims-fraud-detection):** logistic regression with 91.09% recall and 96.99% ROC-AUC on 5,410 providers, using SMOTE for class imbalance.
* **[US County Economic Risk Dashboard](https://github.com/aadityaa-dava/UMBC-DATA606-Capstone) (DATA 606 capstone):** composite risk score for 3,221 counties from Census ACS data, with a live Streamlit app.

---

## Technical Skills

**Languages:** Java, TypeScript, Python, SQL, R

**Backend and APIs:** Spring Boot, NestJS, FastAPI, REST, Kafka, PostgreSQL, Redis, BullMQ

**Data and ML:** PySpark, Spark, Airflow, dbt, Snowflake, Databricks, MLflow, DVC, scikit-learn, LightGBM

**Cloud and DevOps:** AWS (DynamoDB, SNS, Pinpoint), Azure, Docker, Kubernetes, GitHub Actions, Testcontainers, k6, Prometheus, Grafana, OpenTelemetry, Git

**BI:** Tableau, Power BI

---

## Publication

**[Implementing an Accident Detection and Notification System Using AWS](https://www.ijesat.com/ijesat/files/V24I6012_1727765957.pdf)**, IJESAT, Vol. 24, Issue 06, 2024.
Co-author. Built the AWS cloud backend (DynamoDB, SNS, Pinpoint) for an IoT crash detection prototype.

---

## Current Focus

* Full-time SDE roles starting January 2027
* Distributed systems and backend reliability
* Data pipelines and cloud infrastructure

---

## Connect With Me

**Email:** [aadityaa.dava.dev@gmail.com](mailto:aadityaa.dava.dev@gmail.com)

**LinkedIn:** https://www.linkedin.com/in/aadityaa-dava-688908308

**GitHub:** https://github.com/aadityaa-dava
