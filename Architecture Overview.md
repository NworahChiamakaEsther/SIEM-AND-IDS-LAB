# Architecture Overview

## Description
This lab simulates a small enterprise security monitoring architecture with centralized visibility into endpoint and network activity.

---

## Components

### Wazuh Server (Ubuntu)
- Wazuh Manager
- Wazuh Indexer
- Wazuh Dashboard

### Endpoints
- Windows endpoint with Wazuh Agent
- Ubuntu endpoint with Wazuh Agent and Suricata IDS/IPS

---

## Data Flow
1. Endpoints generate system, security, and network logs
2. Wazuh Agents forward logs to the Wazuh Manager
3. Suricata generates IDS alerts on the Ubuntu endpoint
4. Wazuh Indexer stores and indexes all events
5. Wazuh Dashboard visualizes alerts and logs

---

## Security Value
- Centralized monitoring
- Improved detection capabilities
- Audit-ready security logging
- Defense-in-depth architecture
