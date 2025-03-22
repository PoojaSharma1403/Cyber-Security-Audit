# Incident 001 - Phishing Investigation

## Scenario
A user reported a suspicious email. Investigation initiated to determine if it was a phishing attack.

## Tools Used
- Splunk
- Email Header Analysis (Python Script)
- MITRE ATT&CK
- VirusTotal

## Findings
- Email spoofed "From" field using lookalike domain.
- SPF and DKIM failed authentication.
- Link in the email redirected to a credential harvesting page.

## Response
- Blocked sender domain and phishing URL.
- Alerted users via email about the phishing campaign.
- Logged the incident and updated SOC playbook.

## Lessons Learned
- Implement stricter email filtering.
- Train users to spot red flags.
- Automate header analysis for future incidents.
