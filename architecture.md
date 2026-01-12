# SIEM Architecture

## Overview
This lab uses a centralized SIEM architecture where Splunk Enterprise collects and analyzes logs from multiple endpoints using Splunk Universal Forwarders.

---

## Components
- **Splunk Enterprise**
  - Installed on Windows
  - Central log collection and analysis platform
  - Listening on TCP port 9997

- **Log Sources**
  - Windows endpoint (Security Event Logs)
  - Ubuntu Server (SSH authentication logs)
  - Kali Linux (attack simulation and system logs)

---

## Data Flow
Endpoints → Splunk Universal Forwarder → Splunk Enterprise

Logs are forwarded in near real-time for detection and analysis.
