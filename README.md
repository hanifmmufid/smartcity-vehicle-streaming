# SmartCity Vehicle Trip Streaming Pipeline

A real-time data pipeline simulating vehicle trip data for the **Malang-Surabaya route (Indonesia)**. This project generates sensor metrics, weather conditions, and traffic events, streams the data via **Apache Kafka**, and persists it to **Amazon S3** for further analytics.

---

## Features
- **Real-time Data Generation**:
  - Simulates vehicle movement between Malang and Surabaya.
  - Generates GPS data, speed, weather conditions, and traffic events.
- **Streaming with Kafka**:
  - Data is streamed to Kafka topics (`vehicle_data`, `gps_data`, `weather_data`, etc.).
- **Cloud Storage**:
  - Persists data to Amazon S3 using Kafka Connect S3 Sink Connector.
- **Scalable & Modular**:
  - Designed for IoT use cases, traffic analysis, and fleet management.

---

## Tools Used
- **Data Generation**: Python (Faker, UUID, Datetime)
- **Streaming**: Apache Kafka, Confluent Kafka-Python
- **Cloud Storage**: Amazon S3 + Kafka Connect S3 Sink Connector
- **Orchestration**: Docker (for local Kafka/S3 setup)
- **Data Format**: JSON/Avro