# Cyber-Security-Task-1
# 🛡️ Cybersecurity Internship – Task 1: Network Port Scanning with Nmap

## 🔍 Objective:
To perform a TCP SYN scan using Nmap on the local network to identify active hosts and any open ports. This task helps build foundational skills in network reconnaissance and understanding service exposure.

---

## 🛠️ Tools Used:
- **Nmap** (Version 7.97)
- **Operating System**: [Kali Linux in VMware]
- (Optional: Wireshark) 

---

## 📡 Scan Method:
**Command used:**
```bash
nmap -sS 192.168.1.0/24
📊 Scan Summary:
Number of hosts detected as UP: 52

Total IPs scanned: 256

Open ports found: 0

Most common port states: filtered, no-response, net-unreach, time-exceeded

Example IP status:
192.168.1.1: 904 filtered ports, 96 unreachable

192.168.1.4: 773 filtered (time-exceeded), 227 no-response

Others: 1000 filtered ports

🧠 Analysis:
No open ports were detected on any active device.
This indicates that most devices have:

Firewall or port filtering enabled

No exposed services running

Some devices responded to ping or SYN packets but did not allow port access

🔐 Security Insight:
This is a good sign from a network security standpoint — fewer exposed services reduce the attack surface.
However, it could also indicate:

IDS/IPS systems dropping packets silently

NAT/firewall configurations that reject port scans

📁 Files Included:
scan_result1.txt: Raw output of the Nmap scan

README.md: Documentation of the task and analysis

📌 Key Learnings:
How to perform a SYN scan using Nmap

How to interpret filtered vs. open vs. closed ports

The role of firewalls and filters in protecting networks

Network reconnaissance basics


With the help of wireshark I was able to capture real-time packet data to better understand what scanning looks like at networking level
