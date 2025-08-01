# SOC-Analyst-Homelab-Real-World-Threat-Detection-with-Splunk-Sysmon-Zeek-MITRE-ATT-CK
SOC-style homelab simulating real-world detection workflows using Splunk, Sysmon, Zeek, Hydra, Nessus, and MITRE ATT&amp;CK. Built to mirror the tools and techniques used in modern Blue Teams.
# SOC Analyst Homelab: Real-World Threat Detection with Splunk, Sysmon, Zeek, Suricata & MITRE ATT&CK

This homelab simulates a real-world Security Operations Center (SOC) environment, built to practice detection engineering, threat analysis, and incident triage. Using enterprise-grade tools like Splunk, Suricata, Zeek, and Nessus, this project mirrors the tools and techniques used by modern Blue Teams.

---

## Lab Setup

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

### RDP Brute Force Detection
- Executed an RDP brute-force attack from Kali to the Windows 10 VM using Hydra  
- Detected multiple EventCode 4625 login failures  
- Logged and correlated events in Splunk SIEM using Sysmon and Universal Forwarder  
- Mapped detection to MITRE ATT&CK T1110: Brute Force  

### Network-Based Threat Analysis
- Monitored traffic with Suricata to detect known signatures and suspicious payloads  
- Parsed protocol activity using Zeek for post-exploitation insight  
- Verified IDS alerts and correlated them with endpoint events in Splunk  

---

## Why I Built This

To gain practical, job-ready SOC skills by working hands-on with the same toolset used in enterprise environments. This lab simulates real detection workflows, demonstrates deep understanding of adversary behavior, and shows my ability to configure, monitor, and respond to real security events.

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

## Career Relevance

This project is part of my active transition into cybersecurity. It reflects the investigative mindset, tooling familiarity, and detection engineering workflows expected of a Tier 1–2 SOC Analyst or Blue Team role.

Built to continue to expand my skillset. I will continue to add, refine, and perfect, as best I can, these skills to best apply them to my career.

Explore the repo, view screenshots, and follow along as I expand this environment into a full-fledged detection engineering playground.
