# 🎧 Spotify Data Stack Project

Project Overview

This project demonstrates an **end-to-end real-time data engineering pipeline** for **Spotify music analytics** using the **Modern Data Stack (MDS)**.  
We simulate streaming music data — including **song plays, listeners, regions, and device types** — and build a fully automated pipeline from **data ingestion to visualization**.

Once the pipeline starts, **every component runs automatically**:  
data simulation → streaming via Kafka → storage in Snowflake → transformation with DBT → visualization in Power BI.

👉 Think of it as a **real-world Spotify analytics system** built on top of cutting-edge data tools.

## 📂 Repository Structure

```text
spotify-mds-pipeline/
├── docker/ # DAGs for orchestration
│   ├── .env
│   ├── docker-compose.yml
│   └── dags/
│       ├── minio-to-kafka.py
│       └── .env
├── spotify_dbt/
│   └── models/
│       ├── gold/
│       ├── silver/
│       └── sources.yml
├── simulator/
│   ├── producer.py
│   └── .env
├── consumer/
│   ├── kafka-to-minio.py
│   └── .env
├── docker-compose.yml
├── requirements.txt
└── README.md
```
---

