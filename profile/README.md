#  Smart Campus Digital Twin

> A real-time digital replica of a physical campus — integrating IoT sensor data, 3D visualization, and intelligent analytics to monitor, manage, and optimize campus operations.

![Status](https://img.shields.io/badge/Status-In%20Development-yellow?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)

---

## 🌐 Overview

The **Smart Campus Digital Twin** creates a live, data-driven virtual model of a campus environment. It streams real-time sensor data, renders an interactive 3D campus model, and applies machine learning to optimize energy usage, space utilization, and resource management — all in one unified platform.

---

## ✨ Features

- 🗺️ **3D Campus Visualization** — Interactive real-time campus model built with Three.js
- 📡 **IoT Sensor Integration** — Live data from environmental, occupancy, and energy sensors
- ⚡ **Real-time Streaming Simulation** — High-throughput event pipeline via MQTT → Kafka → Apache Flink
- 📊 **Analytics & Reporting** — Batch processing with Apache Spark and workflow automation via Airflow
- 🤖 **ML Intelligence** — Predictive models for energy optimization, attendance, and anomaly detection
- 🏢 **Resource Management** — Monitor energy, attendance, and campus assets in real time


---

## 🛠️ Tech Stack

### Data & Streaming
| Layer | Technology |
|---|---|
| IoT Protocol | MQTT |
| Message Broker | Apache Kafka |
| Stream Processing | Apache Flink |
| Batch Processing | Apache Spark |
| Workflow Orchestration | Apache Airflow |

### Storage
| Purpose | Technology |
|---|---|
| Time-series (sensor data) | InfluxDB |
| Relational (campus data) | PostgreSQL |

### Backend & ML
| Layer | Technology |
|---|---|
| API | FastAPI (Python) |
| Machine Learning | Python / ML Libraries |

### Frontend
| Layer | Technology |
|---|---|
| Language | TypeScript |
| 3D Visualization | Three.js |

---

## 🤝 Contributing

We welcome contributions! Please read our [**CONTRIBUTING.md**](./CONTRIBUTING.md) before opening issues or pull requests.

- Open an issue → assign yourself → branch → PR → review → merge
- Follow conventional commits and branch naming conventions
- Direct pushes to `main` are not allowed

---

## License

This project is licensed under the [MIT License](./LICENSE).

---
