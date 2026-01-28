# Phishing Simulation + SIEM/EDR Mapping (GoPhish)

## Overview
This project demonstrates a complete phishing attack lifecycle using **GoPhish** and maps the activity to **SOC detection and response** concepts including **SIEM**, **EDR**, and **SOAR**.

## What I Built
- Credential-harvesting phishing campaign (GoPhish)
- Landing page for credential capture
- Email template for lure delivery (lab simulation)
- Campaign tracking (open → click → submit)
- SIEM correlation and EDR endpoint visibility mapping
- SOAR response workflow (containment + remediation)
- MITRE ATT&CK alignment (T1566 – Phishing)

## Lab Environment
- Kali Linux (VM)
- GoPhish (local deployment)

## Results
The campaign successfully demonstrated:
- Email opened
- Link clicked
- Credentials submitted
(See screenshots and report.)

## SOC Mapping Summary

### SIEM (Detection & Correlation)
Log sources and high-level correlation:
- Email gateway logs (phishing delivery)
- Web proxy/firewall logs (URL click)
- Application telemetry (credential submission)
- Authentication logs (possible account misuse)

### EDR (Endpoint Visibility)
Endpoint-level signals:
- Browser activity accessing phishing URL
- Credential input behavior
- Suspicious outbound traffic patterns

### SOAR (Automated Response)
- Block phishing URL/domain
- Force password reset
- Notify SOC and create incident ticket
- User awareness follow-up

### MITRE ATT&CK
- **T1566 – Phishing** (Initial Access)
- Credential harvesting activity (Credential Access)



## Disclaimer
This project is for **educational and defensive security learning only** in a controlled environment.
