# Cyber Incident Reporting Toolkit

> A small, practical toolkit for **junior SOC analysts** to report, classify and respond to cybersecurity incidents in a consistent way.

![Status](https://img.shields.io/badge/status-active-brightgreen) ![Type](https://img.shields.io/badge/type-documentation-blue) ![Licence](https://img.shields.io/badge/licence-educational-lightgrey)

## Purpose

Clear, consistent incident reports help a Security Operations Centre (SOC) respond faster, spot trends and prove what happened. This project provides ready-to-use documents that standardise how incidents are written up. It was created as part of a Junior Cybersecurity Analyst assessment for **Zulu Global Inc**.

## What is in this repository?

| Path | Description |
|------|-------------|
| [`templates/incident-report-template.md`](templates/incident-report-template.md) | Blank incident-reporting template to copy for every new incident |
| [`docs/severity-classification.md`](docs/severity-classification.md) | Risk-score ranges and how to classify an incident |
| [`docs/incident-response-checklist.md`](docs/incident-response-checklist.md) | Step-by-step checklist based on the NIST incident response lifecycle |
| [`examples/sample-phishing-incident-report.md`](examples/sample-phishing-incident-report.md) | A fully completed example (fictional data) |
| [`SECURITY.md`](SECURITY.md) | Rules for handling sensitive data in this repository |

## How to use

1. Copy `templates/incident-report-template.md` and rename it using the pattern `INC###-short-description.md` (for example `INC006-phishing-finance-team.md`).
2. Fill in every section. Use the severity guide to choose the risk level.
3. Work through the response checklist while handling the incident and tick items off.
4. Submit the finished report to the SOC lead for review.

## Severity levels at a glance

| Average risk score | Risk level |
|--------------------|-----------|
| 0 – 49 | Minimal |
| 50 – 59 | Low |
| 60 – 69 | Medium |
| 70 – 79 | High |
| 80 and above | Critical |

## Important

All data in this repository is **fictional**. Never commit real passwords, API keys, personal data, customer information or live incident evidence. See [`SECURITY.md`](SECURITY.md).

## Contributing

Suggestions are welcome through issues and pull requests. Use clear commit messages (for example `docs: add ransomware example`) and have changes reviewed before merging.

## References

- NIST SP 800-61 Rev. 2, *Computer Security Incident Handling Guide*
- CISA, *Avoiding Social Engineering and Phishing Attacks*
