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

