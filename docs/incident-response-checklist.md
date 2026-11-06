# Incident Response Checklist

Based on the four phases of the NIST incident response lifecycle (NIST SP 800-61 Rev. 2).

## 1. Preparation

- [ ] Contact list for the SOC and management is up to date
- [ ] Logging and monitoring tools are working
- [ ] Staff have received security-awareness training
- [ ] Incident report template is available to all analysts

## 2. Detection and analysis

- [ ] Record the time of detection and who reported it
- [ ] Confirm whether it is a real incident or a false positive
- [ ] Identify affected systems, accounts and data
- [ ] Score the incident and assign a risk level
- [ ] Preserve evidence (screenshots, logs, email headers) in a secure location
- [ ] Notify the SOC lead if risk level is High or Critical

## 3. Containment, eradication and recovery

- [ ] Isolate affected devices from the network
- [ ] Disable or reset compromised accounts
- [ ] Block malicious domains, IP addresses and email senders
- [ ] Remove malware and close the vulnerability used
- [ ] Restore systems from clean backups
- [ ] Monitor closely after recovery

## 4. Post-incident activity

- [ ] Complete the incident report
- [ ] Hold a lessons-learned review
- [ ] Update procedures, detection rules and awareness material
- [ ] Share relevant findings with affected staff
- [ ] Close the incident ticket
