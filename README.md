
# network-vapt

🔐 Network Vulnerability Assessment & Exploitation – Lab Environment

📌 Project Overview

This project demonstrates a complete Network Vulnerability Assessment and Controlled Exploitation performed in an isolated lab environment using Metasploitable 2 as the vulnerable target system.
The objective was to simulate a real-world security assessment by identifying exposed services, analyzing vulnerabilities, validating critical findings, and recommending remediation strategies.

⚠️ This project was conducted strictly in a controlled lab environment for educational and ethical purposes only.

🎯 Objectives
Perform full network enumeration
Identify open ports and running services
Detect outdated or vulnerable software
Prioritize risks using CVSS scoring
Validate critical vulnerabilities via controlled exploitation
Document findings in a structured security report

🛠 Tools & Technologies Used 
Nmap – Network scanning & service enumeration
Metasploit Framework – Exploitation & validation
Searchsploit – CVE research
Netcat – Manual testing
Kali Linux – Attacker machine
Metasploitable 2 – Vulnerable target machine

🌐 Lab Setup
Component	Details
Target System	Metasploitable 2
Target IP	Internal Lab Network
Attack Machine	Kali Linux
Network Type	Isolated Virtual Lab

🔎 Phase 1 – Network Enumeration
Performed a full TCP scan to identify exposed services:
nmap -sV -O -p- <target-ip>

Identified Services Included:
FTP (Port 21)
SSH (Port 22)
Telnet (Port 23)
SMTP (Port 25)
DNS (Port 53)
HTTP (Port 80)
SMB (Ports 139/445)
PostgreSQL (Port 5432)
VNC (Port 5900)
Apache Tomcat (Port 8180)

🔎 Phase 2 – Vulnerability Assessment
Used OpenVAS to detect:
Outdated service versions
Weak authentication mechanisms
Remote Code Execution vulnerabilities
Exposed database services
Misconfigurations

Vulnerabilities were categorized based on:
CVSS v3 scoring
Exploitability
Impact severity

Severity levels assigned:
Critical
High
Medium
Low

🔎 Phase 3 – Controlled Exploitation
Critical vulnerabilities were validated using Metasploit Framework.

Examples of validated findings:
Samba Remote Code Execution
FTP Backdoor vulnerability
Weak SSH credentials
Exposed PostgreSQL access
VNC weak authentication

Successful exploitation demonstrated:
Remote shell access
Privilege escalation
Database access
Full system compromise (in lab)

📊 Risk Analysis & Impact
The assessment revealed multiple high-risk vulnerabilities that could lead to:
Remote Code Execution
Unauthorized access
Data exfiltration
Privilege escalation
Lateral movement within a network

🛡 Remediation Recommendations
Disable legacy and insecure services (e.g., Telnet, R-services)
Replace FTP with SFTP
Enforce strong authentication policies
Patch outdated software versions
Restrict database exposure to internal networks
Implement firewall segmentation
Enable logging and monitoring for suspicious activity

📄 Documentation
A detailed vulnerability assessment report is included in this repository:
📎 NetworkVAPT.pdf

The report contains:
Technical findings
Exploitation evidence
CVSS-based risk prioritization
Remediation strategies

🎓 Key Learning Outcomes
Practical network enumeration techniques
Vulnerability analysis and CVE research
Risk prioritization using CVSS
Real-world exploitation validation
Security reporting methodology

⚠️ Disclaimer
This project was conducted in a virtual lab environment for educational purposes only.
Unauthorized testing on real-world systems is illegal and unethical.


