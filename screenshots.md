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
<img width="1366" height="768" alt="Screenshot 2026-01-12 002851" src="https://github.com/user-attachments/assets/fdb35332-8c61-4107-843c-159a741374ba" />
<img width="1366" height="768" alt="Screenshot 2026-01-12 002557" src="https://github.com/user-attachments/assets/3b747dae-cd35-4bf9-bb19-26b8e40d85c8" />

### Linux SSH Failed Login Detection

Log source:

- /var/log/auth.log

Detection keyword:

- Failed password

Detection logic:

- Multiple failed SSH login attempts from a single source IP

**Screenshot of Linux SSH failed login detection:**
<img width="1366" height="768" alt="Screenshot 2026-01-12 012515" src="https://github.com/user-attachments/assets/4981a813-c0d9-4c25-9f84-0a368cdf4e3f" />





### Raw Event Analysis

Reviewed _raw event data

Validated:

- Timestamp accuracy

- Source and sourcetype

- Authentication failure messages

**Screenshot of raw event view:**
<img width="1366" height="768" alt="Screenshot 2026-01-12 023636" src="https://github.com/user-attachments/assets/c00c286a-8403-40e7-9f59-755648a24360" />

### Incident Timeline Analysis

Time-based visualization of attack activity

- Identified spike in failed authentication attempts

- Correlated events leading to alert generation

**Screenshot of incident timeline visualization:**
<img width="1366" height="768" alt="Screenshot 2026-01-12 023618" src="https://github.com/user-attachments/assets/8bc13593-a8d5-4665-88dc-8d3e3d40e264" />
<img width="1366" height="768" alt="Screenshot 2026-01-12 023636" src="https://github.com/user-attachments/assets/75dcb776-a303-474c-9bd7-cfa7f649994e" />
<img width="1366" height="768" alt="Screenshot 2026-01-12 023648" src="https://github.com/user-attachments/assets/9f0aeffd-0242-4240-85a0-0138c2b725de" />


### Data Summary Validation

Confirmed successful ingestion of:

- Windows logs

- Ubuntu Server logs

- Kali Linux activity logs

- Verified indexes and sourcetypes in Splunk
**Screenshot of Splunk data summary:**
  <img width="1366" height="768" alt="Screenshot 2026-01-12 011515" src="https://github.com/user-attachments/assets/cc9aff67-4467-4a1a-9a4a-53ae71ebeb4c" />

  <img width="1366" height="768" alt="Screenshot 2026-01-12 011347" src="https://github.com/user-attachments/assets/3b22c0f2-1bd5-4209-83ed-cbda4536e0c0" />

<img width="1366" height="768" alt="Screenshot 2026-01-12 011445" src="https://github.com/user-attachments/assets/04aa37a1-68a5-4970-8a0d-5d5f53b2413f" />

