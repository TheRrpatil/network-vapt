# network-vapt
This project documents a comprehensive vulnerability assessment conducted within a controlled lab environment. The assessment focused on identifying open ports, detecting outdated services, evaluating security risks using CVSS scoring, and providing structured remediation recommendations.
🎯 Objectives

Discover live hosts within the lab network

Identify open ports and running services

Detect vulnerabilities using automated scanning tools

Prioritize findings based on CVSS severity ratings

Recommend actionable remediation steps

🛠 Tools Used

Nmap – Network discovery and port scanning

OpenVAS – Vulnerability assessment and management

Linux (Kali/Ubuntu) – Testing environment

🔎 Methodology
1️⃣ Network Scanning (Nmap)

Performed host discovery

Conducted TCP SYN scans

Identified service versions

Enumerated exposed ports

Example command:

nmap -sS -sV -O 192.168.1.0/24

2️⃣ Vulnerability Scanning (OpenVAS)

Configured and launched full vulnerability scan

Analyzed detected vulnerabilities

Exported scan reports

Reviewed CVSS base scores

3️⃣ Risk Prioritization

Vulnerabilities were categorized as:

🔴 Critical (CVSS 9.0–10.0)

🟠 High (CVSS 7.0–8.9)

🟡 Medium (CVSS 4.0–6.9)

🟢 Low (CVSS 0.1–3.9)

Prioritization was based on:

CVSS score

Exploitability

Impact on confidentiality, integrity, and availability
