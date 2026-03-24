
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

## Setup Instructions
### 1. Clone Repository

git clone https://github.com/idris-yak/global-tech-news-data-pipeline.git
cd global-tech-news-data-pipeline

### 2. Install Dependencies

pip install -r requirements.txt

### 3. Configure AWS Credentials
aws configure

### 4. Start Airflow
airflow standalone

### 5. Trigger DAG
__Open Airflow UI
__Enable tech_news_pipeline
__Trigger DAG manually or wait for scheduled run
__Output__
__Local Output__

