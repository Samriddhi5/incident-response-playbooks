# 📝 Incident Report

**Incident Title:**  
Theft of Backup Tapes Containing Hashed Password Files

**Date of Incident:**  
2025-02-18

**Reported By:**  
Automated alert (Backup Integrity Check System)

---

## 1. Executive Summary

On February 18, 2025, Viva la Vita Online detected the theft of backup tapes from its offsite storage containing `/etc/passwd` and `/etc/shadow` files from a legacy 2015 Linux server. The incident posed a risk of credential exposure and potential customer data compromise.

---

## 2. Timeline of Events

| Time (UTC) | Event Description |
|------------|------------------|
| 10:20      | Alert received on missing backup inventory |
| 10:45      | Manual ticket created in IR platform |
| 11:10      | IR team assembled and containment plan initiated |
| 12:00      | Legacy credentials disabled; short-term monitoring started |
| 15:00      | Root cause analysis began; external authorities notified |

---

## 3. Root Cause Analysis

The stolen backup tapes were inadequately secured and stored without proper encryption. The 2015 server used outdated password hashing algorithms, and physical security protocols at the storage facility had not been recently audited.

---

## 4. Impact Assessment

- **Systems Affected:**  
  2015 backup images of Linux database servers

- **Data Exposure:**  
  Customer credentials (hashed), potential indirect access to order history

- **Business Impact:**  
  Reputational risk; potential regulatory scrutiny under data protection laws

---

## 5. Indicators of Compromise (IOCs)

| Type       | Value                     |
|------------|---------------------------|
| File Names | /etc/passwd, /etc/shadow  |
| Tape IDs   | LTO5-DB01, LTO5-DB02      |

---

## 6. Response Actions Taken

- [x] Disabled credentials from legacy systems
- [x] Notified Legal and PR teams
- [x] Conducted full inventory of all backup tapes
- [x] Deployed increased logging and SIEM alerting
- [x] Initiated encryption policy review for all stored data

---

## 7. Recovery Steps

- Verified system integrity using clean backup images
- Strengthened physical access controls and added MFA for facility access
- Re-validated backup procedures and policies

---

## 8. Lessons Learned

- Physical security needs annual auditing
- Legacy credentials must be purged regularly
- Backup tapes must be encrypted at rest, always

---

## 9. Reporting & Compliance

- **Report Submitted To:**  
  CISO, Legal, and Compliance teams

- **Legal/Privacy Review Completed:**  
  Yes

- **Public Disclosure Required:**  
  Pending legal assessment

---

## 10. Attachments

- 📎 Backup tape audit report  
- 📎 Credential map and expiration status  
- 📎 Updated backup SOP  
- 📎 Root cause analysis summary

---

> *Prepared by:*  
> Alex R.  
> Security Operations Team  
> 2025-02-20
