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
| Desktop PC       | 192.168.1.137 | PC          | Not scanned       |

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

**Operating System:** Linux 3.2 – 3.16  
**Observations:**  
- Router exposed DNS, HTTP, HTTPS, and SIP ports to the internal network.  
- Port 5060 (SIP) may be vulnerable if unused.  
**Next Steps / Recommendations:**  
- Disable SIP (5060) if not using VoIP.  
- Ensure router firmware is updated.  
- Use a strong admin password for router management.

---

### 2. Smartphone (Infinix HOT 10i, 192.168.1.195)
**Open Ports & Services:** None (all 1000 scanned ports closed)  
**Observations:**  
- Device is not exposing any inbound services on the local network.  
- Android default security is effectively blocking external scans.  
**Next Steps / Recommendations:**  
- Periodically review app permissions for outbound connections.  
- Run mobile antivirus/security scans to ensure no malicious apps are present.

---

## Skills Demonstrated
- Network scanning and discovery using **Nmap**  
- Service and version detection on devices  
- OS fingerprinting and basic network profiling  
- Identifying potential vulnerabilities and open ports  
- Writing professional security assessment reports

---

## Conclusion
This project demonstrates foundational **network security skills** applied to real devices:  
- Router analysis revealed actionable security improvements.  
- Mobile device analysis confirmed strong default protection.  
- Provides a practical **portfolio example** showing capability in scanning, analyzing, and recommending security improvements.

