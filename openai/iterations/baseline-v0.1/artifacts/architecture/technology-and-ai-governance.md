# Technology and AI Governance

Iteration: `baseline-v0.1`

Status: `draft`

Module: `MOD-TAI`

## Design Thesis

Technology is governed as civic infrastructure when it affects rights, public services, security, ecological impact, or market concentration. AI may advise and augment public work, but accountable humans and appealable institutions remain responsible for coercive or rights-affecting decisions.

Evidence links: CLM-029, CLM-030, CLM-031, CLM-032, CLM-033.

## AI Use Rules

| Use Class | Rule |
| --- | --- |
| Public benefits triage | AI may assist but cannot make final denial decisions without human review and appeal. |
| Policing and security | High-risk predictive or biometric systems require legislative authorization, impact assessment, warrant-like constraints, and public reporting; some uses may be prohibited. |
| Courts and sentencing | AI may support legal research and administrative scheduling; it must not determine guilt, liability, sentencing, or detention. |
| Public administration | AI may draft, summarize, detect anomalies, and improve service access under audit logs and quality review. |
| Education and health | AI must be assistive, transparent to users, privacy-preserving, and overseen by qualified humans. |
| Governance deliberation | AI may summarize evidence and arguments but must disclose uncertainty, source limits, and alternative interpretations. |

## Data Rights

Baseline rights:

- Notice, access, correction, deletion where compatible with public records law, portability, purpose limitation, minimization, human appeal, and breach notification.
- Public institutions need stricter observability than private persons.
- Civic data trusts may govern shared infrastructure data under fiduciary duties and public audit.

## Technical Safeguards

| Control ID | Control | Related Risk |
| --- | --- | --- |
| TAI-C001 | Mandatory AI impact assessments for public and high-impact private systems. | RSK-010 |
| TAI-C002 | Model and data provenance records. | RSK-010 |
| TAI-C003 | Independent audits and red-team tests before deployment. | RSK-010, RSK-003 |
| TAI-C004 | Appeal and human-review pathway for affected persons. | RSK-010 |
| TAI-C005 | Cybersecurity controls mapped to identify, protect, detect, respond, and recover. | RSK-009 |
| TAI-C006 | Open standards and exit clauses in procurement. | RSK-010 |

## Biosecurity and Dual Use

- Sensitive knowledge transfer and laboratory capabilities require tiered access, audit, ethics review, incident reporting, and international coordination.
- Controls must distinguish legitimate research from dangerous operationalization.

## Open Issues

| Issue ID | Issue | Register |
| --- | --- | --- |
| TAI-O001 | Which biometric and predictive systems should be banned rather than regulated. | CON-006 |
| TAI-O002 | How to audit foundation models whose training data cannot be fully inspected. | ASM-012 |
| TAI-O003 | Balancing open science with biosecurity limits. | CON-007 |
