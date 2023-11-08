# Kafka-Realtime-Streaming

### System Architecture
![](Data%20engineering%20architecture.png)

### Project Overview
This project is building an end-to-end pipeline. Start from ingestion data till final process and storage. And the tech stack in this project used is apeche airflow, apache kafka, apache spark, apache zookeeper and cassandra. Everything is containerized using Docker for ease of deployment and scalability.

### Project designed
1. Data Source: We use randomuser.me API to generate random users data for our pipeline
2. Apache Airflow: Responsible for orchestrating the pipeline and storing fetched data in a PostgreSQL database.
3. Apache Kafka and Zookeeper: Used for streaming data from PostgreSQL to the processing engine.
4. Control Center and Schema Registry: Helps in monitoring and schema management of our Kafka streams.
5. Apache Spark: For data processing with its master and worker nodes.
6. Cassandra: Where the processed data will be stored.