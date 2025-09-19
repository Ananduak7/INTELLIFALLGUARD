# 🛡️ IntelliFallGuard — IoT-Based Fall Detection and Health Monitoring System

**IntelliFallGuard** is an innovative IoT-based system designed to ensure the safety and well-being of elderly individuals.  
It uses **YOLOv5-based computer vision** and **MPU6050 sensor data** to detect falls in real time, while also monitoring key health parameters such as **heart rate, blood oxygen levels, and temperature**.  

The system provides **immediate alerts** to caregivers and features a **web-based dashboard** for real-time monitoring.

---

## 👥 Team Members
- **Anandakrishnan A (21BCE1682)**
- **Mr. Niranjan (21BCE1988)**  

---

## 📋 Problem Statement

Current fall detection systems often:
- Rely on **wearables or pressure sensors** which are intrusive and inconvenient
- Produce **false alarms** from normal movements
- Lack **real-time monitoring** and **health data integration**

**IntelliFallGuard** addresses these issues by using a **non-intrusive, vision+sensor-based hybrid approach** with automated alerts and remote monitoring capabilities.

---

## 🎯 Objectives

- **Accurate fall detection** using YOLOv5-based video analysis
- **Sensor-assisted validation** using MPU6050 acceleration and gyroscope data
- **Real-time alerts** via SMS and email to caregivers

## To be done
- **Health monitoring** of heart rate, SpO2, temperature, and humidity using ESP8266 module and connected sensors
- **User-friendly dashboard** to display camera feed, fall status, and health analytics

---

## ⚙️ System Architecture

### Components
- **Camera Module:** Captures real-time video of the elderly user
- **YOLOv5 Model:** Detects falls from video frames
- **MPU6050 Sensor:** Provides acceleration and gyroscope data for fall detection
- **ESP8266 Wi-Fi Module:** Transmits data to cloud server
- **Cloud Server:** Runs YOLO model, processes sensor data, sends alerts
- **React Web Dashboard:** Shows camera feeds, health data, and fall alerts

---

## 🧩 Workflow

1. **Data Capture**  
   - Camera captures video stream  
   - MPU6050 collects accelerometer and gyroscope data

2. **Processing**  
   - YOLOv5 model analyzes frames for fall patterns  
   - Sensor thresholds or ML model (Random Forest / SVM) validate falls

3. **Alert & Logging**  
   - If fall detected, ESP8266 triggers SMS/email alerts  
   - Data stored in cloud database for analysis

4. **Visualization**  
   - Dashboard shows real-time camera feed, fall status, and health parameters

---


