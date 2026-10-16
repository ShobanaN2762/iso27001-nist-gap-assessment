# 🛡️ Enterprise Cloud Gap Assessment (ISO 27001:2022 & NIST CSF 2.0) & Statement of Applicability (SoA) extract

[![Framework: ISO 27001:2022](https://img.shields.io/badge/Framework-ISO%2027001%3A2022-blue.svg)](https://www.iso.org/standard/27001)
[![Framework: NIST CSF 2.0](https://img.shields.io/badge/Framework-NIST%20CSF%202.0-green.svg)](https://www.nist.gov/cyberframework)
[![Regulation: DPDP Act 2023](https://img.shields.io/badge/Regulation-DPDP%20Act%2023-orange.svg)](https://www.meity.gov.in/)
[![Illustrative Score: 50.0%](https://img.shields.io/badge/Compliance%20Score-50.0%25-yellow.svg)](#-executive-compliance-dashboard)

> **Note:** This is a portfolio project. The company (VortexPe Cloud Services), interviews, and findings are fictional and simulated using a persona-based approach. No real systems or data were assessed.

## 📌 Executive Overview
This repository contains a simulated enterprise-level **Information Security Gap Assessment**, **Statement of Applicability (SoA) extract**, and **30-60-90 Day Risk Remediation roadmap** for **VortexPe Cloud Services**—a fictional cloud-native SaaS fintech platform operating on AWS and Kubernetes (EKS).

The engagement evaluated Ten sample enterprise cloud infrastructure and security controls against **ISO/IEC 27001:2022 (Annex A)**, **NIST CSF 2.0**, and the Indian **Digital Personal Data Protection (DPDP) Act 2023** considering personal data findinigs.

## 📊 Compliance Summary

| Item | Result |
|---|---|
| Controls sampled | 10 |
| Applicable and scored | 9 |
| Inherited from AWS, not scored | 1 (A.7.1, data-centre physical security) |
| Fully / Partially / Not implemented | 2 / 5 / 2 |
| Illustrative score | 50.0% = (2 × 1.0 + 5 × 0.5) / 9 |
| Risk ratings (all 10 sampled) | Critical 2, High 4, Medium 1, Low 3 (including 1 inherited control) |

The score is a simple weighting for demonstration. ISO 27001 does not define a compliance percentage.

## 🔍 Critical and High Findings

| # | Finding | Risk | ISO 27001:2022 | NIST CSF 2.0 |
|---|---|---|---|---|
| 1 | Unmasked customer PII in staging | Critical | A.8.12 (primary), A.8.11, A.8.33 | PR.DS-01 |
| 2 | DR failover untested | Critical | A.5.29 (also A.5.30) | ID.IM-02 |
| 3 | No MFA on AWS CLI/API access | High | A.8.5, A.5.15 | PR.AA-03 |
| 4 | Container image signatures not enforced | High | A.8.9 | PR.PS-05 |

## 📂 Repository Structure

```text
iso27001-nist-gap-assessment/
├── README.md                          <-- Portfolio homepage (Includes project context & methodology)
├── 01_Gap_Assessment_and_SoA_Matrix.xlsx <-- 13-column evaluation sheet + dynamic Excel dashboard
├── 01_Company_Context_and_Scope.pdf  <-- Document 1: Company Profile, Scoping & Audit Methodology
├── 02_Statement_of_Applicability.pdf <-- Document 2: Formal ISO 27001 Annex A SoA
└── 03_Executive_Gap_Analysis_Report.pdf <-- Document 3: Board-level Gap Analysis & 30-60-90 Roadmap
```

## ⚠️ Limitations

- Only 10 controls were sampled. A full SoA covers all 93 Annex A controls.
- Findings come from simulated persona interviews, not real evidence testing.
- Maturity ratings and the score are illustrative.
- Proposed RTO/RPO values should be validated through a business impact analysis.
- Control and framework mappings reflect my judgment as a learner and are open to feedback.
