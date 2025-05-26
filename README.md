# Task-1-Elevate_labs
Discover open ports on devices in your Local network to understand network exposure

# CYBER SECURITY INTERNSHIP - TASK 1  
**Network Port Scanning with Nmap**  

---

## 🔍 Objective  
Discover open ports on devices in the local network to assess network exposure and security risks.

---
## Prerequisites
1.Stable Network Connection
2.kali system (I am using Orcale VM Virtual Box)

## 🛠️ Tools Used  
- **Nmap** (`-sS` SYN Scan, Version Detection)   
- **GitHub** (Documentation & Submission)  

---

## 📝 Steps 
1. **Determined Local IP Range**  
   - Command: `ip addr` (Linux) /  
   - Identified subnet: `10.0.2.15/24`.  

2. **Performed TCP SYN Scan**  
   ```bash
   nmap -sS -sV -T4 -oN TCP_scan.txt -oX TCP_scan.xml 10.0.2.0/24
