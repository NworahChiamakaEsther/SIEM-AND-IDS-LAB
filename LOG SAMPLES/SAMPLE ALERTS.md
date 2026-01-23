# Sample Security Alerts & SOC Triage Walkthrough

This section demonstrates how alerts from Wazuh and Suricata would be handled in a real SOC environment.

---

## Alert 1: Multiple Failed Login Attempts (Windows)

**Source:** Wazuh Agent – Windows  
**Severity:** Medium  

### Triage Process
- Review username and timestamps
- Check source IP (internal vs external)
- Correlate with successful login attempts

### Decision
- Monitor if internal and limited
- Escalate if repeated or external

**GRC Value:** Access control monitoring and audit evidence

---

## Alert 2: Suspicious Process Execution (Ubuntu)

**Source:** Wazuh Agent – Ubuntu  
**Severity:** Medium–High  

### Triage Process
- Identify process and executing user
- Validate against expected admin activity

### Decision
- Investigate unknown processes
- Escalate if persistence indicators exist

**GRC Value:** System integrity and least privilege enforcement

---

## Alert 3: Network Scan Detected (Suricata)
<img width="332" height="101" alt="attack_simulation" src="https://github.com/user-attachments/assets/6beff161-ed6d-47f0-8cb6-687b350d1c8f" />


**Source:** Suricata IDS 
**Severity:** High  
<img width="827" height="82" alt="suricata_alert" src="https://github.com/user-attachments/assets/84390ab5-9b7e-4ffc-aa90-2361038b79b1" />


### Triage Process
- Review source IP and ports scanned
- Determine internal vs external origin

### Decision
- Block malicious IPs
- Escalate as confirmed security event

**GRC Value:** Network security monitoring

---

## Correlation Example
Multiple alerts across IDS and endpoint logs increase confidence and justify escalation.

---

