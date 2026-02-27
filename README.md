🚨 Intrusion Detection System (IDS) Using Python & Scapy
📌 Description

This Intrusion Detection System (IDS) monitors network traffic in real-time to identify suspicious activities and potential security threats.

It leverages the powerful Scapy library to capture and analyze network packets, detecting abnormal patterns such as:

Unusually large packets

Repetitive traffic patterns

Potential flood attacks

When anomalies are detected, the IDS can automatically take preventive actions — such as blocking suspicious IP addresses using Windows Firewall commands.

All detected threats and system events are logged for further analysis and review.

✨ Features
📡 Real-time Packet Monitoring

Captures and analyzes network packets in real-time using Scapy.

📊 Statistical Analysis

Tracks packet sizes and frequency.

Identifies unusual traffic patterns.

🚩 Anomaly Detection
📦 Large Packet Detection

Flags packets larger than 1500 bytes as potentially malicious.

🔄 Repetitive Traffic Detection

Detects repetitive packet sizes occurring more than 100 times.

Helps identify possible flood attacks.

🚫 Automated Response

Blocks offending IP addresses using Windows Firewall commands.

⚠ Requires Administrator privileges.

📝 Logging

Logs all detected threats in ids_logs.log.

Includes:

Timestamp

Source IP

Type of anomaly detected

🔔 Alerting (Extendable)

Logging system enables easy integration of:

Email alerts

SMS notifications

Dashboard monitoring

🛠 Technologies Used

🐍 Python – Core programming language

📡 Scapy – Packet capture and analysis

🧱 Windows Firewall – IP blocking mechanism

🎯 Ideal For

🧑‍💻 Network Security Professionals

🕵️ Security Researchers

🧑‍🎓 Python Developers learning network security

🛡 Cybersecurity Students exploring IDS concepts

🚀 How to Run
1️⃣ Clone the Repository
git clone <repo-url>
cd <repository-folder>
2️⃣ Install Required Dependencies
pip install scapy
3️⃣ Run the IDS (Admin Privileges Required)
python ids.py

💡 On some systems:

python3 ids.py

⚠ Make sure to run the terminal as Administrator, otherwise firewall blocking will not work.

📂 Log File

All alerts and detections are saved in:

ids_logs.log

You can analyze this file for:

Attack patterns

Suspicious IP addresses

Traffic anomalies
