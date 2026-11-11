# Sentinel-AI
SentinelAI is a machine-learning-based network intrusion detection system (NIDS). Its purpose is to analyze network traffic and identify connections that may represent suspicious or potentially malicious activity.

Imagine a college network with hundreds of computers, phones, and servers connected to the internet. Every time a device communicates with another device, network traffic is generated.

**Most of this traffic is normal. However, some traffic may be associated with:**
- Port scanning, where someone probes a system for open ports.
- Denial-of-service (DoS) attacks, which attempt to overwhelm a service.
- Brute-force attempts, where someone repeatedly tries to guess login credentials.
- Unusual connections that could indicate compromised devices.
SentinelAI will analyze records describing this traffic and use machine learning to flag patterns that deserve further investigation.

Important: SentinelAI will be a defensive analysis tool. It will work with recorded network traffic datasets or uploaded traffic records, not secretly monitor devices or automatically block anyone.

**What happens when someone uses the website?**
1. The user opens SentinelAI in a browser.
2. They upload a network traffic CSV file.
3. The frontend sends the file to the Python backend.
4. The backend preprocesses the data and runs the trained models.
5. The models return classifications, anomaly scores, and risk estimates.
6. The backend sends the results to the frontend.
7. The website displays the results through charts, alerts, and detailed reports.
This makes the project a proper web application, not just a dashboard mockup.

**Technologies Used:**

Frontend — HTML, CSS, JavaScript
Creates the website's layout, navigation, interactive elements, upload forms, and dashboard.

Backend — Python + Flask
Handles website requests, file uploads, data processing, and communication with the machine learning models.

Machine Learning — scikit-learn
Runs Isolation Forest and Random Forest to analyze network traffic.

Charts — Chart.js
Displays traffic trends, threat categories, and model performance.

Database — SQLite
Stores alert history, analysis summaries, and relevant metadata.

**What's included :**
- Live Monitor: Capture packets from an authorized network interface.
- Dataset Replay: Upload a CSV and process its records continuously.
- ML Detection: Isolation Forest anomaly detection and Random Forest classification.
- Live Dashboard: Automatic event updates, severity counts, and threat feed.
- Event Stream: Search and filter detected events.
- Reports: Download event data as JSON.
