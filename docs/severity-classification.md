# Severity Classification Guide

Each incident is scored from **0 to 100** in three threat categories: **Phishing**, **Malware** and **Unauthorised Access**. The **average risk score** (the mean of the three) is mapped to a risk level.

## Risk levels

| Range start | Risk level | Typical response |
|-------------|-----------|------------------|
| 0  | Minimal  | Log and monitor |
| 50 | Low      | Investigate within 3 working days |
| 60 | Medium   | Investigate within 1 working day |
| 70 | High     | Investigate immediately; notify SOC lead |
| 80 | Critical | Escalate immediately; activate the incident response team |

## Quick status rule

An incident with an average risk score of **60 or above** is flagged **High Risk**; anything below 60 is **Low Risk**. This matches the spreadsheet formula `=IF(G2>=60,"High Risk","Low Risk")` used in the SOC workbook.

## Worked example

| Phishing | Malware | Unauthorised access | Average | Level |
|---------:|--------:|--------------------:|--------:|-------|
| 65 | 72 | 58 | 65.0 | Medium |

## Spreadsheet lookup

In Excel the level can be found with an approximate-match lookup:

```
=VLOOKUP(G2, LookupData!$A$2:$B$6, 2, TRUE)
```

The `$` signs (absolute references) keep the lookup table fixed when the formula is copied down.
