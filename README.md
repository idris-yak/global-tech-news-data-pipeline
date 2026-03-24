
# Global Tech News Data Pipeline

## Overview
This project implements an automated data pipeline that collects, processes, and stores technology news using the Hacker News API. The pipeline is orchestrated using Apache Airflow and stores processed data in Amazon S3 for downstream analytics.

## Business Context
Technology analysts require up-to-date insights on:
- Emerging technology trends
- Product launches
- High-engagement tech discussions

Manual data collection is inefficient. This pipeline automates the process and provides structured data for analysis.

## Pipeline Architecture
1. Extract: Fetch top 20 stories from Hacker News API
2. Transform: Clean and structure relevant fields
3. Load: Store processed data in Amazon S3

## Technologies Used
- Python
- Apache Airflow
- Amazon S3
- Pandas
- Boto3

## Project Structure
global-tech-news-data-pipeline/
│
├── dags/
│   └── tech_news_dag.py
│
├── scripts/
│   ├── extract.py
│   ├── transform.py
│   └── load.py
│
├── data/
│   └── (generated files)
│
├── requirements.txt
└── README.md

