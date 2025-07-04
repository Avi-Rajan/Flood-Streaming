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

