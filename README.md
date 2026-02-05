🔐 SOC Traffic Analysis & Threat Detection
📌 Project Overview

This project simulates a Security Operations Center (SOC) analytics workflow by analyzing web traffic logs to identify potentially malicious IP behavior. Using Python for data analysis and Power BI for visualization, the project demonstrates how security teams can prioritize threats based on traffic patterns, anomaly scores, and threat indicators.

The goal is not hacking, but security monitoring and decision support using data.

🎯 Problem Statement

Organizations receive large volumes of web traffic every day. Manually reviewing logs to identify suspicious activity is inefficient and error-prone.

This project answers key SOC questions:

Which IPs generate unusually high traffic?

Which IPs have abnormal behavior based on anomaly scores?

Which IPs have been flagged as threats?

How can we prioritize IPs for investigation?

🧰 Tools & Technologies

Python (pandas)

Power BI

CSV-based security log data

📂 Dataset Description

The dataset contains simulated web traffic logs with the following fields:

IP_Address – Source IP of the request

Request_Type – HTTP request method (GET, POST, etc.)

Response_Time_ms – Server response time

Anomaly_Score – Score indicating abnormal behavior (0–1)

Is_Threat – Threat label (1 = threat, 0 = normal)

🔍 Analysis Workflow
1️⃣ Data Exploration

Verified dataset structure and data types

Analyzed distribution of request types and response times

Examined anomaly score behavior and threat labels

2️⃣ IP-Level Aggregation

Logs were aggregated at the IP level to create SOC-relevant metrics:

Total request count per IP

Average anomaly score per IP

Total threat events per IP

This produced a clean, investigation-ready table.

🚦 Detection Logic
Rule-Based Detection

An IP was flagged as suspicious if any of the following conditions were met:

High request volume

High average anomaly score

One or more threat flags

Risk Scoring

A weighted risk score was created to prioritize alerts:

Request volume

Anomaly severity

Threat frequency

Each IP was classified into:

Low Risk

Medium Risk

High Risk

📊 Power BI Dashboard

A SOC-style Power BI dashboard was built to support investigation workflows:

Dashboard Features:

KPI cards showing total IPs and suspicious IPs

Table of IPs with risk level and security metrics

Bar chart highlighting high-risk IP traffic

Scatter plot comparing anomaly score vs request volume

The dashboard enables quick identification of IPs requiring attention.

📈 Key Insights

A small number of IPs generate a disproportionately high number of requests

High anomaly scores often correlate with increased threat flags

Risk scoring improves prioritization compared to binary threat labels

✅ Project Outcome

Produced BI-ready security datasets

Built SOC-style detection logic using explainable rules

Created an interactive Power BI dashboard for threat monitoring

Demonstrated practical cybersecurity analytics skills

Because the dataset contains limited repeated IP activity, traffic volume was less informative. The analysis therefore focused on anomaly severity and threat frequency, which are commonly used SOC indicators when volume signals are weak.

🚀 Skills Demonstrated

Security log analysis

SOC-style threat detection

Rule-based risk modeling

Data aggregation and feature engineering

Power BI dashboard design

📌 Next Steps

Integrate time-based analysis (hourly / daily trends)

Tune detection thresholds

Expand to authentication or network flow logs

👤 Author

Emiliano Sandoval
Aspiring SOC / Cybersecurity Data Analyst
