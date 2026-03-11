🔐 SOC Traffic Analysis & Threat Detection
📘 Project Description

This project analyzes web traffic logs to identify potentially suspicious IP addresses. It simulates a simplified Security Operations Center (SOC) workflow used to monitor network activity and detect possible threats.

The analysis was done using Python for data processing and Power BI for visualization.

🛠 Tools Used

Python (pandas) – data cleaning and analysis

Power BI – dashboard and visualization

CSV dataset – simulated security logs

🔎 Analysis Process
📥 Data Exploration

The dataset was explored to understand its structure and key variables:

IP_Address – source of the request

Request_Type – type of HTTP request

Response_Time_ms – server response time

Anomaly_Score – score indicating unusual behavior

Is_Threat – indicates whether a request was flagged

📊 IP-Level Aggregation

To make the data easier to analyze, requests were grouped by IP address.
For each IP, the following metrics were calculated:

Total number of requests

Average anomaly score

Number of threat events

🚨 Detection Logic

IPs were considered suspicious if they showed:

High request volume

High anomaly scores

One or more threat flags

Each IP was then classified into a risk level: Low, Medium, or High.

📈 Dashboard

A Power BI dashboard was created to visualize the results, including:

Total and suspicious IP counts

IP table with risk levels

Charts showing anomaly scores and traffic patterns

This allows quick identification of IPs that may require investigation.

👤 Author

Emiliano Sandoval
Aspiring Cybersecurity / SOC Data Analyst
