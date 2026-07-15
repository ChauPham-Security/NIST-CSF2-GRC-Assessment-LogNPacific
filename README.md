# NIST-CSF2-GRC-Assessment-LogNPacific
End-to-end GRC project — NIST CSF 2.0 gap assessment, risk register, and incident response plan for a live Azure-hosted platform

# NIST CSF 2.0 GRC Assessment — Log(N) Pacific

**Type:** End-to-end GRC engagement  
**Framework:** NIST Cybersecurity Framework 2.0  
**Assessor:** Chau Pham, CISSP  
**Date:** July 2026  

---

## Overview

This is a complete GRC engagement conducted for Log(N) Pacific, a cloud-hosted cybersecurity training platform built on Microsoft Azure. The assessment was performed against a live production environment — not a simulation or lab exercise — and the final deliverables were reviewed and accepted by Josh Madakor, owner of Log(N) Pacific.

The scope covers the company as a whole, including the Azure tenant, Entra ID, Microsoft Sentinel, Defender for Endpoint, Tenable, and the admin team's operational practices. Evidence was gathered from the Cyber Range Architecture and Engineering Document, direct responses from the business owner, publicly available platform information, and live inspection of the Azure environment.

---

## Deliverables

| File | Description |
|------|-------------|
| `NIST_CSF2_GapAssessment_LogNPacific.xlsx` | Full assessment workbook — maturity scores across 100+ controls, 20-entry risk register, dashboard, and remediation document register |
| `LogNPacific_NIST_CSF2_ExecutiveSummary.docx` | Executive summary — key findings, priority risk table, and recommended next steps written for a non-technical business owner |
| `LogNPacific_RS001_IncidentResponsePlan.docx` | Incident Response Plan — formal IRP based on NIST SP 800-61, covering the full incident lifecycle from detection through post-incident review |

---

## What the Assessment Covered

The assessment evaluated Log(N) Pacific's security posture across all six NIST CSF 2.0 functions:

- **Govern** — governance structure, risk appetite, policy ownership, and oversight cadence
- **Identify** — asset inventory, privileged account management, and threat modeling
- **Protect** — identity lifecycle, access control, MFA enforcement, and data protection
- **Detect** — monitoring coverage, detection sources, and alert management
- **Respond** — incident classification, escalation paths, containment, and eradication procedures
- **Recover** — recovery architecture, communication procedures, and lessons learned process

---

## Key Findings

**Critical (Score 12)**
- Two accounts hold Global Administrator access beyond what their function requires — the automation service principal and an account tied to a personal email identity. A compromised Global Administrator gives an attacker full, unrestricted control over the Azure tenant.

**Medium (Score 9)**
- No formal Incident Response Plan existed to cover the full lifecycle of a company-level incident. The business owner had strong working knowledge of NIST SP 800-61 and had applied it successfully in practice, but the process had not been written down for consistent use by the rest of the team. This gap was remediated as part of this engagement.

**Medium (Score 9)**
- No scheduled review of real threat activity against the management plane. Detection relies on Defender for Endpoint, UEBA, and MFA — a proportionate choice for the environment — but no cadence exists to confirm this posture remains appropriate as threats evolve.

The complete risk register with all 20 entries, likelihood and impact scores, owners, and treatment decisions is in the assessment workbook.

---

## Overall Maturity Snapshot

| Function | Avg Maturity Score | Controls Assessed | Controls Below Target |
|----------|-------------------|-------------------|----------------------|
| GV — Govern | 2.5 | 15 | 7 |
| ID — Identify | 2.7 | 12 | 4 |
| PR — Protect | 3.0 | 19 | 6 |
| DE — Detect | 2.2 | 11 | 6 |
| RS — Respond | 2.1 | 12 | 10 |
| RC — Recover | 2.6 | 7 | 3 |
| **Overall** | **2.5** | **76** | **36** |

Target maturity: 3.0 across all functions.

---

## What I Took Away From This Project

GRC work is not about finding every possible gap. It is about understanding the environment well enough to know which gaps actually matter, and communicating that clearly to someone who has to make decisions with limited time and resources. Proportionality and business context matter as much as technical accuracy. Writing "Risk Accepted" is a fundamentally different decision from writing "Closed" — and knowing the difference is what separates a real assessment from a checklist exercise.

**Key skills applied:**

NIST CSF 2.0 control assessment against live evidence, risk scoring and register development, executive communication, policy authorship based on NIST SP 800-61, and cross-referencing technical findings against business context to produce proportionate, actionable recommendations.

---

## Tools and Frameworks Referenced

`NIST CSF 2.0` `NIST SP 800-61` `Microsoft Azure` `Microsoft Sentinel` `Defender for Endpoint` `Entra ID` `Tenable` `KQL` `DISA STIG` `MITRE ATT&CK`

---

## About the Assessor

**Chau Pham | CISSP** — Security professional specializing in governance, risk, and compliance with hands-on technical depth across Azure, Sentinel, and Tenable.

- LinkedIn: [linkedin.com/in/chaupham01](https://www.linkedin.com/in/chaupham01/)
- GitHub: [github.com/ChauPham-Security](https://github.com/ChauPham-Security)
- Email: chaupham.career@gmail.com
