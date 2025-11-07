# FUTURE_CS_02
# Security Incident Detection and Analysis Using Splunk SIEM

**Project:** SOC Simulation — Splunk Enterprise  
**Intern:** Hari Rakesh Yengantiwar  
**Program:** Future Interns – Cybersecurity Internship

---

## Overview
This project demonstrates a Security Operations Center (SOC) simulation using Splunk Enterprise on Windows 11.  
It covers log ingestion, searching, alert triage, visualization, and incident reporting.

## Contents
- `SOC_Final_Report.docx` — Full project report and findings.  
- `splunk.mp4` — Demo video (10:08) showing the steps and screenshots.  
- `screenshots/` — Screenshots used in the report (1.png ... 11.png).  
- `scripts/voiceover_script.txt` — Voice-over script for the video.  
- `.gitattributes` — Git LFS settings (if used).  
- `.gitignore` — Ignored files.

> **Note:** If `splunk.mp4` is large, it is tracked with Git LFS. If not using LFS, the video is hosted externally and a link will be provided here.

## How to reproduce / run
1. Install Splunk Enterprise on Windows (local setup).  
2. From Splunk UI, use *Add Data* → *Upload files from my computer* to ingest:
   - `Application.txt`
   - `syslog.txt`
   - `Network Logs.txt`
   - `auth.log`  
3. Use the **Search & Reporting** app to run queries shown in screenshots and create visualizations.

## Key Findings
- Firewall rule modification — High severity  
- Multiple failed login attempts — High severity  
- Unrecognized USB driver detected — Medium severity  
- Repeated application errors — Low severity

## Recommended actions
- Verify firewall changes were authorized; reset if suspicious.  
- Investigate failed login source IPs and enable account lockout.  
- Remove unauthorized drivers and inspect devices.  
- Investigate application errors for tampering/crashes.

## License
This repository is released under the [MIT License](LICENSE).

## Contact
Hari Rakesh Yengantiwar — _Future Interns_  
