# 🚨 Intrusion Detection System (IDS) Using Python & Scapy

## 📌 Description

This Intrusion Detection System (IDS) monitors network traffic in real-time to identify suspicious activities and potential threats.

It uses the **Scapy** library to capture and analyze network packets, looking for abnormal patterns such as unusually large packets or repetitive requests. Upon detecting anomalies, the IDS can take automated preventive actions, such as blocking suspicious IP addresses using Windows Firewall commands.

All detected threats and system events are logged for further analysis and review.

---

## ✨ Features

### 📡 Real-time Packet Monitoring
- Captures and analyzes network packets in real-time using Scapy.

### 📊 Statistical Analysis
- Tracks packet sizes and counts to identify unusual traffic patterns.

### 🚩 Anomaly Detection

#### 📦 Large Packet Detection
- Flags packets larger than **1500 bytes** as potentially malicious.

#### 🔄 Repetitive Traffic Detection
- Detects repetitive packet sizes (more than 100 times) that may indicate a flood attack.

### 🚫 Automated Response
- Blocks offending IP addresses using Windows Firewall commands.
- Requires **Administrator privileges**.

### 📝 Logging
- Logs all detected threats to `ids_logs.log`.
- Includes timestamps and anomaly details.

### 🔔 Alerting (Extendable)
- Logging system can be extended to trigger:
  - Email notifications
  - SMS alerts
  - Dashboard monitoring

---

## 🛠 Technologies Used

- **Python** – Core programming language
- **Scapy** – Network packet manipulation and analysis
- **Windows Firewall** – Used for blocking suspicious IP addresses

---

## 🎯 Ideal For

- Network Security Professionals
- Security Researchers
- Cybersecurity Students
- Python Developers learning network security concepts

---

## 🚀 How to Run

### 1️⃣ Clone the Repository

```bash
git clone <repo-url>
cd <repository-folder>
2️⃣ Install Required Dependencies
pip install scapy
3️⃣ Run the Program (Administrator Required)
python ids.py
```
Or:
```
python3 ids.py

```
⚠ Make sure to run the terminal as Administrator, otherwise firewall blocking will not work.

📂 Log File

All alerts and detections are saved in:
```
ids_logs.log
```
You can review this file to analyze:

Suspicious IP addresses

Attack patterns

Traffic anomalies
