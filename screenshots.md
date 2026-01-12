## Alert Configuration

- Alerts configured as **Scheduled Searches**
- Trigger condition:
  - Multiple failed login attempts within a defined time window
- Alert Type:
  - Per Result
- Severity:
  - Medium

**Screenshot of triggered alerts:**
<img width="1366" height="768" alt="Screenshot 2026-01-10 092545" src="https://github.com/user-attachments/assets/870f7b1c-15c4-456d-aa3a-e3861c14d5dc" />

## Dashboard Visualization

Created dashboards to provide SOC analysts with:
- Source IP of attack
- Number of failed attempts
- Affected hosts
- Time-based visualization of attack activity

**Dashboard view:**
<img width="1366" height="768" alt="Screenshot 2026-01-10 093032" src="https://github.com/user-attachments/assets/b1fc4c6e-329e-4039-a364-2187c64a2ebd" />

### Kali Attack Simulation

Attack platform:

- Kali Linux

Attack technique:

- SSH brute-force simulation

Purpose:

- Generate malicious authentication events

- Validate SIEM detections and alerts

**Screenshot of Kali attack activity:**
<img width="1366" height="768" alt="Screenshot 2026-01-10 093701" src="https://github.com/user-attachments/assets/72d080ef-712e-456b-ae25-db88d597db7f" />

### Windows Failed Login Detection

Log source:

- Windows Security Event Log

Event ID:

- 4625 (Failed logon)

Detection focus:

- Repeated failed authentication attempts

- Suspicious login behavior

**Screenshot of Windows failed login detection:**
