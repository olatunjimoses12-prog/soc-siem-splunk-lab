# Detections

## Windows Failed Login Detection
Detects multiple failed login attempts on Windows systems.

- Event ID: 4625
- Detection Logic:
  - Count failed logins per account and IP
  - Identify suspicious authentication behavior

---

## Linux SSH Brute Force Detection
Detects repeated failed SSH authentication attempts.

- Log Source: auth.log
- Detection Logic:
  - Match "Failed password"
  - Aggregate attempts by source IP
  - Trigger on threshold breach
