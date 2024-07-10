# Stock Market Kafka Real Time Data Engineering Project

This project demonstrates the use of Apache Kafka for real-time data streaming and processing.

## Introduction
In this project, I executed an End-To-End Data Engineering Project on Real-Time Stock Market Data using Apache Kafka. This project showcases how Apache Kafka can be used to handle real-time data streams. In this project, we simulate a stock market data feed, produce this data to Kafka topics, and consume the data from these topics for processing and analysis.

## Architechture
![Architecture Diagram](Architecture.jpg)

## Technologies Used
- **Programming Language**: Python
- **Amazon Web Services (AWS)**:
  1. S3 (Simple Storage Service)
  2. Athena
  3. Glue Crawler
  4. Glue Catalog
  5. EC2
- **Apache Kafka**

## Dataset Used
For this project, I used a stock market dataset. While the primary focus is on the operational aspects of Data Engineering, you can use any dataset. Here is the dataset I used: [indexProcessed.csv]

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/AshaRavilla/stock-market-kafka-data-engineering-project.git
    ```
2. Navigate to the project directory:
    ```bash
    cd stock-market-kafka-data-engineering-project
    ```

## Setup

### Prerequisites

- Java 8 or later
- Apache Kafka 3.7.1
- Zookeeper 3.7.1

### Starting Zookeeper and Kafka

1. Start Zookeeper:
    ```bash
    bin/zookeeper-server-start.sh config/zookeeper.properties
    ```

2. Start Kafka broker:
    ```bash
    bin/kafka-server-start.sh config/server.properties
    ```

## Usage

### Producing Data

Use the following command to start a producer:
```bash
bin/kafka-console-producer.sh --topic demo_test --bootstrap-server <your_kafka_server>:9092
Consuming Data
Use the following command to start a consumer:
bin/kafka-console-consumer.sh --topic demo_test --bootstrap-server <your_kafka_server>:9092
