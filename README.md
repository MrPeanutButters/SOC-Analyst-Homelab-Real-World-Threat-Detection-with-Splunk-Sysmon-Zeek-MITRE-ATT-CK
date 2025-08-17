# 🛡️ SOC Analyst Homelab: Real-World Threat Detection with Splunk, Sysmon, Zeek, Suricata & MITRE ATT&CK  

This homelab simulates a real-world Security Operations Center (SOC) environment, built to practice detection engineering, threat analysis, and incident triage. Using enterprise-grade tools like Splunk, Suricata, Zeek, and Nessus, this project mirrors the tools and techniques used by modern Blue Teams.  

---

## Lab Setup  

![Lab Screenshot](https://github.com/user-attachments/assets/f0dcd576-08c9-4317-8f78-d3b0fd7ad311)  

| Role | Tool | Description |
|------|------|-------------|
| SIEM | Splunk Enterprise | Ingests and correlates logs from endpoint and network data sources |
| Endpoint Logging | Sysmon + Windows Event Logs | Collects telemetry from Windows 10 victim |
| Network Detection | Zeek & Suricata (via Security Onion) | Deep packet inspection, IDS alerts, and protocol analysis |
| Attack Simulation | Hydra (Kali Linux) | Simulates brute-force attacks over RDP |
| Vulnerability Scanning | Nessus Essentials | Discovers misconfigurations and exploitable CVEs |
| Framework | MITRE ATT&CK | Used to map detection to real-world TTPs |

---

## Simulated Scenarios  

### 🔑 RDP Brute Force Detection  
- Executed an RDP brute-force attack from Kali to the Windows 10 VM using Hydra  
- Detected multiple EventCode 4625 login failures  
- Logged and correlated events in Splunk SIEM using Sysmon and Universal Forwarder  
- Mapped detection to **MITRE ATT&CK T1110: Brute Force**  
![Brute Force GIF](https://github.com/user-attachments/assets/8accb8a5-146a-4fcd-870b-8e6d7511df47)  

### 🌐 Network-Based Threat Analysis  
- Monitored traffic with Suricata to detect known signatures and suspicious payloads  
- Parsed protocol activity using Zeek for post-exploitation insight  
- Verified IDS alerts and correlated them with endpoint events in Splunk  

---

## ✅ Results & Investigation Workflow  

- **Detection:** Splunk correlation searches flagged repeated failed logins in under **30 seconds**  
- **Validation:** Cross-checked Sysmon logs and Suricata alerts to confirm brute-force activity  
- **Escalation Decision:** Classified as a valid brute-force incident, escalated for remediation  
- **Documentation:** Produced SOC-style incident report with evidence, MITRE mapping, and response steps  

This workflow mirrors how Tier 1/2 SOC analysts operate: detect → validate → escalate → document.  

---

## Skills & Tools Demonstrated  

- SIEM Administration (Splunk)  
- IDS/IPS configuration and alerting (Suricata)  
- Network forensics & analysis (Zeek)  
- Endpoint visibility and logging (Sysmon, Event Viewer)  
- Brute force and credential attack detection (Hydra)  
- CVE detection and remediation workflow (Nessus Essentials)  
- Threat mapping with MITRE ATT&CK  
- Detection engineering and alert rule creation  
- Incident triage and investigation workflows  

---

## Roadmap / Next Steps  

- Simulate malware execution and test Suricata signatures  
- Add detection rules using Sigma/YARA  
- Ingest Suricata alerts into Splunk for central correlation  
- Expand with EDR tools like Wazuh or Velociraptor  
- Develop playbooks for specific attack patterns  

---

## 🎯 Career Relevance  

This project demonstrates I can already perform the **core responsibilities of a SOC analyst**: building detections, triaging alerts, validating incidents, and documenting workflows. It proves I can:  

- Operate SIEMs and IDS/IPS to detect and respond to attacks  
- Align investigations to frameworks like **MITRE ATT&CK**  
- Deliver actionable, low-noise alerts and professional incident documentation  

I built this environment to sharpen the exact skills required on a SOC floor. It shows I can contribute from **day one** as a Tier 1–2 SOC Analyst and continue to grow into more advanced detection engineering and blue team roles.  

---
