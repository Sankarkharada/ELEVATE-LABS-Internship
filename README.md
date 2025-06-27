<<<<<<< HEAD
# Task 4: Setup and Use a Firewall on Linux (UFW)

## 🎯 Objective
Configure and test basic firewall rules on a Linux system using UFW (Uncomplicated Firewall) to control inbound traffic.

---

## 🛠️ Tools Used
- **Operating System**: Kali Linux / Ubuntu
- **Firewall Tool**: UFW (Uncomplicated Firewall)
- **Terminal Commands** (with `sudo` privileges)

---

## 📋 Task Steps

### ✅ Step 1: Check UFW Status
```bash
sudo ufw status verbose
✅ Step 2: Enable UFW
bash
Copy
Edit
sudo ufw enable
✅ Step 3: List Current Rules
bash
Copy
Edit
sudo ufw status numbered
✅ Step 4: Block Inbound Traffic on Port 23 (Telnet)
bash
Copy
Edit
sudo ufw deny 23
✅ Step 5: Test the Rule
Try connecting to port 23 locally (must have telnet installed):

bash
Copy
Edit
telnet localhost 23
You should see: "Connection refused" or similar message.

✅ Step 6: Allow SSH (Port 22)
bash
Copy
Edit
sudo ufw allow 22
✅ Step 7: Remove the Test Block Rule (Port 23)
bash
Copy
Edit
sudo ufw delete deny 23
✅ Step 8: Disable UFW (optional - restore state)
bash
Copy
Edit
sudo ufw disable
📁 Project Files
File	Description
ufw-commands.txt	All terminal commands used
ufw-rules.txt	Output of current firewall rules
screenshots/rules-listed.png	Screenshot showing UFW rule list
README.md	This documentation file

🧠 Summary: How UFW Filters Traffic
UFW is a frontend for iptables, simplifying Linux firewall rule management.

It filters incoming and outgoing network packets based on rules.

Rules can allow or deny traffic based on:

Ports (e.g., 22 for SSH, 23 for Telnet)

IP addresses (optional)

Protocols (TCP/UDP)

Default policy usually denies incoming traffic and allows outgoing traffic, unless explicitly changed.

📷 Screenshots Included
rules-listed.png: Shows firewall rules applied using sudo ufw status numbered

=======
# 🚀 Elevate Labs Cybersecurity Internship Projects

## 📅 Internship Duration
**June 2025 – July 2025**

## 🏢 Organization
**Elevate Labs**

## 👨‍💻 Intern: Sankar Kharada  
Cybersecurity | Network Security | Threat Analysis | Kali Linux

---

## 📘 Overview

This repository contains the tasks completed during my Cybersecurity Internship with **Elevate Labs**, focused on vulnerability assessment, phishing investigation, and network scanning.

Each task folder contains:
- Tools used
- Steps performed
- Reports and screenshots
- Key findings and remediations

---

## 📂 Completed Tasks

### ✅ Task 1: Network Port Scanning
- Performed local network scan using **Nmap**
- Identified open ports and services on active devices
- [View Task](./task-1-network-port-scan/README.md)

---

### ✅ Task 2: Phishing Email Analysis
- Analyzed a phishing email for spoofing and malicious intent
- Used header analyzers and manual inspection
- [View Task](./task-2-phishing-email-analysis/README.md)

---

### ✅ Task 3: Vulnerability Scan using Nessus
- Installed **Nessus Essentials** on Kali Linux
- Ran full scan on localhost and documented vulnerabilities
- Suggested security fixes for top findings
- [View Task](./task-3-vulnerability-scan-nessus/README.md)

---

## 🎯 Skills Gained

- 🔍 Network Enumeration & Scanning
- 🧠 Email Threat Detection
- 🛡️ Vulnerability Assessment
- 📊 Report Writing & Documentation
- 💻 Linux and Cybersecurity Tooling (Kali Linux, Nessus, Nmap)

---

## 📌 Note
All work was performed in a safe lab environment using virtual machines and simulated samples. No real-world exploitation was done.

---

## 📧 Contact
**Sankar Kharada**  
[LinkedIn](https://www.linkedin.com/in/sankarkharada) | Cybersecurity Enthusiast | Red Team Projects Contributor  
>>>>>>> ec1ed7eecb3ca3813066004f8202dfad3d7573ad
