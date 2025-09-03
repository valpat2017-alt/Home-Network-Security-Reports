# Home-Network-Security-Reports
My first project as a network administrator, I did security scan on my home network. This network has three devices connected together (Router, Laptop and Android phone), each device was scanned with Nmap tool.

# Home Network Security Assessment

**Project Overview**  
**Title:** Home Network Security Assessment Using Nmap  
**Date:** September 2025  
**Tools Used:** Nmap (v7.98), Windows 11 Laptop, Android Phone (Infinix HOT 10i), Home Router (Guangzhou Tozed Kangwei)  
**Objective:** Assess the security posture of a home network, identify open ports and services, and analyze potential vulnerabilities for mitigation.

---

## Devices Assessed

| Device Name       | IP Address     | Device Type | MAC Address                        |
|------------------|---------------|-------------|-----------------------------------|
| Home Router      | 192.168.1.1   | Router      | 98:A9:42:28:96:23                 |
| Infinix HOT 10i  | 192.168.1.195 | Smartphone  | 6E:40:D8:47:E8:AC                  |
| Desktop PC       | 192.168.1.137 | PC          | Not scanned for this example       |

---

## Methodology

1. **Network Discovery:**  
   - Ran `nmap -sn 192.168.1.0/24` to discover active devices on the home network.

2. **Service Detection:**  
   - Used `nmap -sV <IP>` to identify open ports and running services on each device.

3. **OS Fingerprinting:**  
   - Used `nmap -O <IP>` to detect the operating system where possible.

4. **Aggressive Scan:**  
   - Applied `nmap -A <IP>` to combine service detection, OS detection, and traceroute.

5. **Documentation:**  
   - Recorded all results, analyzed open ports, and suggested mitigation strategies.

---

## Results

### 1. Home Router (192.168.1.1)
**Open Ports & Services:**
