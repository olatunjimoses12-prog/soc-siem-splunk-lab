# Incident Report – Linux SSH Brute Force

## Summary
A brute-force SSH attack was detected against an Ubuntu Server through repeated failed login attempts.

---

## Timeline
- Failed SSH logins observed in logs
- Detection triggered in Splunk
- Alert reviewed by SOC analyst
- Attacking IP identified

---

## Impact
- No successful authentication observed
- Attack limited to failed attempts

---

## MITRE ATT&CK
- T1110 – Brute Force

---

## Recommendations
- Enforce SSH key-based authentication
- Implement account lockout policies
- Monitor and block malicious IPs
