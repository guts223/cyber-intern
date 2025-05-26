# cyber-intern
Day 1
🔍 Nmap Local Network Scan – Lab Report
📁 Description
This project demonstrates a basic TCP SYN port scan of a local virtual network using Nmap, conducted from a Kali Linux virtual machine running in VMware. The goal is to identify active devices and open ports within an internal test environment to understand network exposure and service enumeration.

🧰 Tools Used
🛠️ Nmap 7.95

🐧 Kali Linux (VM)

🧪 (Optional) Wireshark for traffic capture

📊 What’s Inside
File	Description
sanitized_scan.html	Cleaned-up Nmap scan results, safe for public sharing
scan.xml (optional)	Raw XML output from Nmap (not included here)
README.md	You are here – explains the project

📝 Scan Summary
Scan Range: 192.168.x.0/24 (Virtual Lab)

Hosts Found: 4

Open Ports:

192.168.x.2: Port 53 (DNS) – open

Others: All ports either filtered or closed

🔐 Disclaimer
This scan was performed in a safe, isolated lab environment using private IP addresses on a virtual network. No external systems were scanned. All identifying information (IPs, MACs) has been anonymized for privacy.
📌 Usage
To run a similar scan:
nmap -sS -oX scan.xml 192.168.x.0/24
xsltproc scan.xml -o scan.html
