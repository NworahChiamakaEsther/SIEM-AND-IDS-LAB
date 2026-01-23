# Suricata IDS/IPS Integration

## Objective
Enhance detection capabilities with network-based IDS/IPS.

---

## Steps Performed
- Installed Suricata on Ubuntu endpoint

<img width="758" height="199" alt="suricata_installed" src="https://github.com/user-attachments/assets/c23bd50a-2e49-4b6e-99b4-01bd3a451672" />


- Enabled IDS/IPS monitoring
- Configured Suricata logs to forward to Wazuh

<img width="419" height="80" alt="suricata_config" src="https://github.com/user-attachments/assets/0835d87b-9c94-48ad-90c8-33d7d65e88dd" />


---

## Validation
- IDS alerts generated successfully

<img width="827" height="82" alt="suricata_alert" src="https://github.com/user-attachments/assets/15a9ded6-733a-40d1-a439-97f7e7cfc597" />

- Alerts indexed and displayed in Wazuh Dashboard

<img width="668" height="404" alt="suricata_events_in_wazuh" src="https://github.com/user-attachments/assets/a540788f-d141-4b4d-80c0-8da74fefc2ce" />


---

## Security Value
- Network threat detection
- Complements host-based monitoring
- Supports defense-in-depth
