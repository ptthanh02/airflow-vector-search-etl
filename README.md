# 🚀 Airflow Vector Search Pipeline

## Project Overview

This project implements a robust data pipeline for intelligent document search, leveraging modern technologies to create a seamless information retrieval system.

### Key Technologies
- Apache Airflow
- MongoDB
- QdrantDB (Vector Database)
- Python
- Docker Compose

## 🌟 Features

- Automated data ingestion pipeline
- Vector-based semantic search
- Scalable microservices architecture
- Easy deployment with Docker

## 🛠 Prerequisites

- Docker
- Docker Compose
- Python 3.9+

## 🚦 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/intelligent-document-search.git
cd intelligent-document-search
```

### 2. Load Docker Images
```bash
docker load -i mongo.tar
docker load -i qdrant.tar
docker load -i postgres.tar
docker load -i redis.tar
docker load -i python3911.tar
```

### 3. Start the Data Pipeline
```bash
cd PhamTienThanh_12345678
docker compose up --build
```

## 🔍 Access Points

- **Airflow UI**: http://localhost:8080
  - Username: airflow
  - Password: airflow

- **QdrantDB Dashboard**: http://localhost:6333/dashboard

- **MongoDB Compass Connection**:
  - URL: mongodb://localhost:27017
  - Username: admin
  - Password: admin

## 📝 Pipeline Workflow

The Airflow DAG performs the following steps:
1. Initialize collection in QdrantDB
2. Insert random data into MongoDB
3. Transfer data to QdrantDB
4. Count and verify data
5. Perform vector-based search