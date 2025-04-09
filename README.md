# 🛡️ Incident Response Playbooks

This repository contains structured and actionable security incident response playbooks developed for realistic scenarios in modern enterprise environments. Each playbook outlines key roles, tools, procedures, and post-incident activities based on NIST 800-61 standards and blue team best practices.

---

## 📚 Contents

### 1. 📁 [playbooks/](./playbooks)

| Incident Type                    | Description |
|----------------------------------|-------------|
| 🧷 **Hashed Passwords Theft**     | Response plan for stolen backup tapes containing sensitive hashed passwords (`/etc/passwd`, `/etc/shadow`). Focuses on containment, forensics, and recovery in Linux environments. |
| 📡 **Rogue Wireless Access Point** | Incident response for unauthorized AP detected within a corporate office. Covers identification, physical and network containment, and mitigation against lateral movement. |

### 2. 🧰 [templates/](./templates)
- **HashedPasswords_Incident_Report.md**
- **RogueWiFiAP_Incident_Report.md**

---

## 🛠️ Tools & Technologies Referenced

- 🔍 SIEM: IBM QRadar  
- 🚦 EDR: Symantec Endpoint Protection  
- 🌐 IDS/IPS: Suricata  
- 🔐 Encryption: BitLocker  
- 🔬 Forensics: EnCase, FTK, Autopsy  
- 🔧 Vulnerability Management: Tenable Nessus  
- 🧱 Firewall: Fortinet FortiGate  
- ☁️ Communication: Microsoft Teams, Outlook  

---

## 🔁 Use Case

These playbooks can be used by:
- Security teams to improve readiness
- IR tabletop exercises
- SOC analysts onboarding material
- Security engineering process documentation

---

## ✍️ Author

**Samriddhi**  
Threat Detection Enthusiast  
[LinkedIn](https://www.linkedin.com/in/samriddhi5/)

---

> “Preparedness is not just about having tools — it’s about having a plan to use them when it matters most.”
