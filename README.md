# Nmap Local Network Port Scan

## **Objective**
The goal of this project is to perform a TCP SYN scan on my local network using Nmap to discover open ports and understand potential security risks.

---

## **Tools Used**
- **Nmap** – For scanning the network and identifying open ports.
- **Wireshark** *(optional)* – For packet capture and analysis.
- **Kali Linux** – Running commands and saving results.
- **GitHub** – For storing and sharing results.

---

## **Steps Followed**

### 1. Identify Local IP Range
- Checked IP address and subnet mask using:
```bash
ifconfig

nmap -sS 192.168.0.0/24
nmap -sS 192.168.0.0/24 -oN scan_results.txt
nmap -sS 192.168.0.0/24 -oX scan_results.xml
xsltproc scan_results.xml -o scan_results.html


Optional Packet Analysis

Used Wireshark to monitor SYN packets sent during the scan.
