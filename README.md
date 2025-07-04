# 🌊 Flood-Streaming

A real-time data streaming pipeline simulating flood sensor events using **Apache Kafka**, **AWS EC2**, **Kafka Connect**, and **Amazon S3** — all provisioned via **CloudFormation** with custom **Python** scripts for producers and consumers.

---

## 📌 Project Overview

Flood-Streaming is a fully cloud-native, fault-tolerant streaming data pipeline designed to simulate and process real-time sensor data related to flood monitoring. The system ingests events from simulated IoT devices, publishes them to Kafka, processes and optionally transforms the messages, and ultimately streams them to Amazon S3 for long-term storage and future analytics.

---

## 🎯 Objectives

- Simulate IoT-based flood sensors pushing real-time data.
- Set up a reliable streaming pipeline with Kafka and Kafka Connect.
- Stream incoming data to Amazon S3 using the Kafka S3 Sink Connector.
- Provide modular Python-based producer and consumer scripts.
- Build reproducible infrastructure using AWS CloudFormation.

---

## 🏗️ Architecture

- **Producer**: Publishes JSON events (sensor ID, location, water level, timestamp)
- **Kafka Broker**: Routes data to appropriate topic(s)
- **Kafka Connect**: Reads from topic and streams events into S3
- **Consumer**: Python app for real-time processing (alerting/validation)
- **S3**: Data lake for storing raw or transformed events

---

## 🧰 Tech Stack

| Tool               | Role                                                |
|--------------------|-----------------------------------------------------|
| **AWS EC2**         | Hosts Kafka, Kafka Connect, and Python services     |
| **AWS S3**          | Stores streaming data files                         |
| **AWS CloudFormation** | Provisions networking, EC2, IAM roles, etc.       |
| **Apache Kafka**    | Messaging backbone                                  |
| **Kafka Connect**   | Streams data into S3 (sink connector)               |
| **Python**          | Custom producer and consumer apps                   |
| **AWS EMR (optional)** | Post-stream batch analytics                       |

---
