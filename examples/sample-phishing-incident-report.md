# Incident Report – INC001 (Sample – fictional data)

## 1. Incident summary

| Field | Details |
|-------|---------|
| Incident ID | INC001 |
| Date/time detected | 2026-03-02 09:14 (UTC+2) |
| Date/time reported | 2026-03-02 09:20 (UTC+2) |
| Reported by | Finance department employee |
| Handled by (analyst) | Junior SOC Analyst |
| Incident category | Phishing |
| Status | Resolved |

## 2. Description

Three finance staff received an email that appeared to come from the IT helpdesk asking them to "verify their mailbox" through a link. One employee entered their credentials on a fake login page before realising the website address was unusual and reporting it.

## 3. Risk assessment

| Category | Risk score (0–100) |
|----------|--------------------|
| Phishing | 65 |
| Malware | 72 |
| Unauthorised access | 58 |
| **Average risk score** | **65.0** |
| **Risk level** | **Medium** |

## 4. Affected assets

- Systems / hosts: corporate email, one workstation
- User accounts: 1 account (initials only: T.M.)
- Data involved: mailbox contents (type only)

## 5. Timeline of events

| Time | Event | Source |
|------|-------|--------|
| 08:55 | Phishing email delivered to 3 users | Mail gateway log |
| 09:05 | One user submits credentials on fake page | User report |
| 09:20 | User reports email to SOC | Helpdesk ticket |
| 09:35 | Account disabled and password reset | SOC action |
| 10:10 | Sender domain blocked, emails purged | SOC action |

## 6. Actions taken

- [x] Containment: compromised account disabled, malicious domain blocked
- [x] Eradication: phishing emails removed from all mailboxes, sessions revoked
- [x] Recovery: password reset, multi-factor authentication confirmed, account monitored for 7 days

## 7. Root cause

A convincing phishing email passed the mail filter and the user did not check the link address before entering credentials.

## 8. Recommendations and lessons learned

1. Run a short phishing-awareness refresher for the finance team.
2. Enforce multi-factor authentication on all accounts.
3. Add the look-alike domain and similar patterns to mail-filter rules.
