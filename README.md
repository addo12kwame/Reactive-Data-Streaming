
# Real-Time Data Monitoring Pipeline

This project implements a scalable, real-time data processing pipeline that collects information from YouTube, processes it, and triggers notifications for significant changes. The pipeline leverages **Apache Kafka** for data streaming and **Telegram** for alerting, and can be easily extended to support additional APIs and notification systems.

## 📈 Pipeline Overview

### 1. Data Collection
- **Python scripts** fetch data from external APIs (currently using the YouTube API).
- Designed to support multiple APIs by abstracting the data collection layer.

### 2. Data Ingestion
- Data is ingested into **Apache Kafka** topics for real-time streaming.
- Kafka provides scalability, fault tolerance, and high throughput.

### 3. Stream Processing
- Kafka Streams or custom Python consumers process the data in real-time.
- The system detects significant changes or events based on predefined rules.

### 4. Alerting System
- When changes meet certain criteria, alerts are sent using **Kafka Connect**.
- Notifications are pushed to **Telegram**, with support for additional platforms (e.g., Slack, Email).

## 🛠️ Technologies Used
- **Python**: Scripting for API data collection.
- **Apache Kafka**: Distributed event streaming platform.
- **Kafka Streams**: For real-time stream processing.
- **Kafka Connect**: For integrating with external systems like Telegram.
- **Telegram Bot API**: For sending real-time alerts.

