# 📦 Triminds ObjectScanner

![Platform](https://img.shields.io/badge/Triminds-Platform-blue)
![Computer Vision](https://img.shields.io/badge/AI-Computer%20Vision-success)
![YOLOv8](https://img.shields.io/badge/YOLOv8-Ultralytics-red)
![Android](https://img.shields.io/badge/Android-Native-brightgreen)
![Python](https://img.shields.io/badge/Python-Flask-blue)
![Oracle](https://img.shields.io/badge/Oracle-Database-red)
![License](https://img.shields.io/badge/License-MIT-yellow)
![detector](https://github.com/user-attachments/assets/37645298-c6ae-4051-8510-b6c02c6d69dc)



![detector](https://github.com/user-attachments/assets/37645298-c6ae-4051-8510-b6c02c6d69dc)



## Enterprise Computer Vision Platform for Warehouse Automation

**Triminds ObjectScanner** is an enterprise-grade AI-powered computer vision solution designed to identify, classify and count warehouse assets using standard Android devices.

Instead of relying on expensive specialized hardware, users can scan pallets, boxes, labels, QR Codes, barcodes, and warehouse objects directly from a smartphone. Captured information is processed locally or in the cloud using Artificial Intelligence and automatically integrated with enterprise systems.

---

# 🌐 Part of the Triminds Platform

Triminds ObjectScanner is one of the products within the **Triminds Platform** ecosystem.

Although it can operate as a standalone application, it is designed to integrate seamlessly with the **Triminds Platform UI**, sharing a common architecture, authentication, design system and user experience across the entire platform.

## Related Triminds Projects

| Project                    | Description                                                                                   |
| -------------------------- | --------------------------------------------------------------------------------------------- |
| **Triminds Platform UI**   | Enterprise frontend, Design System and application shell shared across all Triminds products. |
| **Triminds Security**      | Enterprise Authentication, Authorization and Security services.                               |
| **Triminds Geo AI**        | Geospatial Artificial Intelligence platform for Earth Observation and satellite imagery.      |
| **Triminds SmartImageLab** | AI laboratory for image processing, experimentation and computer vision.                      |

### Platform Vision

```text
                    Triminds Platform

                           │

     ┌──────────────┬──────────────┬──────────────┐
     │              │              │              │
 Platform UI   ObjectScanner   Geo AI    SmartImageLab
     │
     └──────────────┬──────────────┐
                    │
               Security Services
```

The Triminds ecosystem follows a modular architecture where products remain independent while sharing a unified enterprise platform.

---

# 🚀 Project Overview

Triminds ObjectScanner combines an Android application with a Python backend to provide real-time object detection, counting and inventory support powered by Artificial Intelligence.

The solution integrates modern Computer Vision techniques with enterprise cloud technologies, enabling organizations to automate warehouse operations without specialized scanning hardware.

---

# ✨ Key Features

* 📱 Native Android application
* 🤖 YOLOv8 real-time object detection
* 🔍 Automatic object counting
* ☁ Azure Computer Vision fallback
* 🏭 Warehouse asset identification
* 📦 Pallet and box recognition
* 🏷 Label and barcode detection
* ☁ Cloud synchronization
* 🗄 Oracle Database integration
* 🔄 REST API
* 🧠 Custom AI model training
* 📊 Audit trail support
* 🔐 Enterprise-ready architecture

---

# 🏗 Solution Architecture

```text
                    Android Device
                           │
                     Camera Capture
                           │
                           ▼
               Image Processing Pipeline
                           │
            ┌──────────────┴──────────────┐
            │                             │
       YOLOv8 Engine         Azure Computer Vision
            │                             │
            └──────────────┬──────────────┘
                           ▼
                    Flask REST API
                           │
        ┌──────────────────┼──────────────────┐
        │                  │                  │
   Oracle Database      Cloud Sync      TLP Integration
```

---

# 📁 Project Structure

```text
ObjectScanner/

├── PythonBackend/
│   ├── app.py
│   ├── requirements.txt
│   ├── setup_en.sh
│   ├── .env.example
│   │
│   ├── ml_model/
│   │   ├── train.py
│   │   ├── detect.py
│   │   ├── export.py
│   │   ├── config.py
│   │   └── dataset/
│   │
│   ├── services/
│   │   ├── object_count_service.py
│   │   ├── ml_detection_service.py
│   │   └── azure_service.py
│   │
│   └── config/
│       └── db_config.py
│
├── Android/
│   ├── app/
│   ├── build.gradle
│   └── settings.gradle
│
├── OracleDatabase/
│   └── schema/
│       └── create_tables.sql
│
├── docs/
│   ├── ADRs/
│   └── architecture.md
│
├── .github/workflows/
│
├── README.md
│
└── .gitignore
```

---

# 🛠 Technology Stack

| Layer             | Technologies                         |
| ----------------- | ------------------------------------ |
| Mobile            | Java, Android SDK, CameraX, Retrofit |
| Backend           | Python, Flask                        |
| AI / ML           | YOLOv8, Ultralytics, Roboflow        |
| Computer Vision   | Azure Computer Vision                |
| Database          | Oracle Database                      |
| Cloud             | Oracle Cloud, Railway, Docker        |
| CI/CD             | GitHub Actions                       |
| Frontend Platform | Triminds Platform UI                 |

---

# ⚙ Core Components

## 📱 Android Application

* CameraX integration
* Image capture
* REST communication
* Offline-ready architecture
* Mobile-first experience

---

## 🤖 AI Detection Engine

* YOLOv8 inference
* Custom datasets
* Roboflow integration
* Object counting
* Bounding box generation
* Confidence filtering

---

## ☁ Azure Vision Integration

When confidence is below the configured threshold, ObjectScanner automatically invokes Azure Computer Vision as a secondary inference engine, increasing robustness in challenging environments.

---

## 🗄 Database Layer

* Oracle Database
* Scan history
* Audit logs
* Detection metadata
* Historical analytics

---

## 🔄 REST API

The backend exposes REST endpoints for inference, model integration and synchronization with enterprise systems.
