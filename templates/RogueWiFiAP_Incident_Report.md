# 📝 Incident Report

**Incident Title:**  
Rogue Wireless Access Point Detected in Cafeteria

**Date of Incident:**  
2025-03-10

**Reported By:**  
Employee ticket submitted via Helpdesk

---

## 1. Executive Summary

On March 10, 2025, employees reported unstable wireless connectivity in the cafeteria. Investigation revealed an unauthorized access point (AP) impersonating Viva la Vita's Wi-Fi network. The rogue AP posed a risk of credential harvesting and traffic interception.

---

## 2. Timeline of Events

| Time (UTC) | Event Description |
|------------|------------------|
| 08:45      | Employee ticket submitted reporting slow Wi-Fi |
| 09:10      | Network team confirmed rogue SSID in proximity |
| 09:30      | AP physically located and disabled |
| 10:00      | IR team initiated log analysis and containment checks |
| 13:00      | Post-incident review began |

---

## 3. Root Cause Analysis

The rogue AP was likely a device brought in by an external contractor. Wi-Fi MAC filtering and WIDS/WIPS controls were not enforced in the cafeteria area.

---

## 4. Impact Assessment

- **Systems Affected:**  
  Guest and corporate Wi-Fi networks (localized)

- **Data Exposure:**  
  Potential credentials if users connected and entered passwords

- **Business Impact:**  
  Low to medium — no confirmed data theft, but high reputational concern

---

## 5. Indicators of Compromise (IOCs)

| Type       | Value                     |
|------------|---------------------------|
| SSID       | VivaLaVita-Free           |
| MAC Addr   | 00:14:22:01:23:45         |
| Channel    | 6                         |

---

## 6. Response Actions Taken

- [x] Rogue AP disconnected and confiscated
- [x] SIEM logs analyzed for unusual activity
- [x] Employees warned via internal communication
- [x] WIDS and MAC filtering enforced in cafeteria zone
- [x] Policies updated for contractor Wi-Fi usage

---

## 7. Recovery Steps

- Restored safe access via official APs
- Verified DHCP logs and endpoint connection history
- Monitored traffic for further anomalies

---

## 8. Lessons Learned

- Wireless IDS needs better alerting thresholds
- Physical checks are still vital in segmented zones
- Awareness training for employees can improve early detection

---

## 9. Reporting & Compliance

- **Report Submitted To:**  
  CISO, IT Director

- **Legal/Privacy Review Completed:**  
  Yes

- **Public Disclosure Required:**  
  No

---

## 10. Attachments

- 📎 Wireless scan logs  
- 📎 Floor plan with rogue AP location  
- 📎 Policy update document  
- 📎 Detection rule adjustments

---

> *Prepared by:*  
> Samriddhi 
> Security Engineer – Detection Team  
> 2025-03-11
