# Risk Register

Artifact ID: ART-030
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: all
Depends on: ART-006

## Purpose

Consolidate operational risks across the framework, scoring likelihood and impact, identifying owners, current mitigations, and residual exposure. Distinct from but built on the failure-mode register (ART-006), which catalogs threat patterns. This register turns those threats into trackable risks tied to specific artifacts and bodies.

## Scoring

Likelihood (1-5): 1 rare, 5 near-certain.
Impact (1-5): 1 minor, 5 catastrophic.
Composite = L × I (range 1-25).
Residual = composite after mitigation.

## Risk Table

| Risk ID | Risk | Source RSK / SCN | Likelihood | Impact | Composite | Mitigation | Residual | Owner | Status |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| REG-001 | Adversarial-review body itself captured or starved | RSK-001, RSK-023; SCN-001 | 3 | 5 | 15 | Mixed-body appointment; constitutional budget floor; constitutional-court protection | 10 | GOV-B5 + constitutional court | Open |
| REG-002 | Sortition bodies fail to sustain legitimacy at scale | RSK-043; SCN-019 | 3 | 4 | 12 | Mixed bodies; compensated service; expert pool; protected from intimidation | 8 | GOV-B1, GOV-B6 | Open |
| REG-003 | Constitutional court packed or coerced | RSK-002, RSK-030; SCN-002, SCN-013 | 2 | 5 | 10 | Mixed-body nomination; non-renewable terms; public reasoning; impeachment threshold high | 6 | GOV-B3 | Open |
| REG-004 | Universal floor real value erodes under inflation | SCN-016 | 3 | 4 | 12 | Cost-of-living indexing; commons protection; macroprudential discipline | 8 | Central bank, Executive Council | Open |
| REG-005 | Capital flight on aggressive wealth taxation | SCN-017 | 3 | 3 | 9 | International cooperation; exit-friction instruments; phased implementation | 6 | Treasury, foreign-affairs | Open |
| REG-006 | Ecological caps breached by political-economy default | SCN-005, SCN-020; RSK-006 | 3 | 5 | 15 | Constitutional ceilings; future-generations advocate; criminal liability for ecocide | 10 | Future-gen advocate, regulators | Open |
| REG-007 | Cyber attack cascading across critical infrastructure | RSK-008; SCN-007 | 3 | 5 | 15 | Redundancy; air-gap discipline; mandatory standards; CSIRT | 9 | TAI-A3 cyber agency | Open |
| REG-008 | AI capability outpaces governance | RSK-010; SCN-008 | 4 | 4 | 16 | Risk-tier classification; audits; international coordination; prohibitions on Tier 1 uses | 12 | TAI-A1 AI regulator | Open |
| REG-009 | Election integrity compromised by AI-enabled manipulation | RSK-020, RSK-042; SCN-008 | 3 | 5 | 15 | Algorithmic-transparency; watermarking; public-service media; algorithmic audits | 10 | Electoral commission, TAI-A1 | Open |
| REG-010 | Foreign invasion or coercion | RSK-011; SCN-009 | 1-3 | 5 | 5-15 | Civil defense; alliances; conventional deterrence; energy and food sovereignty | varies | Defense, foreign-affairs | Open |
| REG-011 | Pandemic exceeds surge capacity | RSK-007; SCN-006 | 3 | 5 | 15 | Preparedness; surge capacity; reserved manufacturing; international cooperation | 9 | Public health | Open |
| REG-012 | Demographic-care collapse | RSK-013, RSK-027; SCN-010 | 3 | 3 | 9 | Care-economy investment; immigration; productivity through automation | 6 | Social-affairs, immigration | Open |
| REG-013 | Despair-meaning crisis deepens | RSK-014; SCN-011 | 3 | 4 | 12 | Mental-health infrastructure; community design; meaningful-work policy; pluralism | 9 | Health, community | Open |
| REG-014 | Crisis-power ratchet entrenches emergency measures | RSK-035, RSK-002; SCN-012 | 3 | 4 | 12 | Hard sunsets; supermajority renewal; judicial review; adversarial-review | 7 | GOV-B5, constitutional court | Open |
| REG-015 | Coup or self-coup | RSK-030; SCN-013 | 1 | 5 | 5 | Civilian control of military; constitutional-court independence; multi-body emergency rules | 3 | All institutions | Open |
| REG-016 | Observability creep into personal surveillance | RSK-009, RSK-034; SCN-014 | 3 | 4 | 12 | Cryptographic separation; member access logs; adversarial-review audits | 8 | TAI-A2 data authority | Open |
| REG-017 | Mob-pluralism collapse via social-media amplification | RSK-037; SCN-015 | 3 | 3 | 9 | Platform-amplification regulation; due-process culture; legal-remedy | 7 | TAI-A1, courts | Open |
| REG-018 | Cooperative sector cannot reach scale | ECO-MK2 risk | 3 | 2 | 6 | Tax treatment; conversion financing; federation support | 4 | Economy | Open |
| REG-019 | Mental-health workforce shortage persists | HEA-W workforce risks | 4 | 4 | 16 | Public funding of education; service obligations; pay competitiveness; task-shifting | 11 | Health, education | Open |
| REG-020 | Tax-administration capacity insufficient for new instruments | ECO-T risks | 3 | 3 | 9 | Phased rollout; international cooperation; capacity-build; beneficial-ownership transparency | 6 | Treasury | Open |
| REG-021 | Public-service media captured or defunded | RSK-002 vector | 2 | 4 | 8 | Constitutional funding floor; arms-length governance; independent funding board | 5 | GOV-B10, public-service media | Open |
| REG-022 | Judicial independence eroded over time | RSK-002, RSK-019 | 2 | 5 | 10 | Mixed-body nomination; tenure protection; salary protection; impeachment threshold | 6 | Constitutional court | Open |
| REG-023 | Migration shock exceeds reception capacity | RSK-012; SCN-005 | 3 | 4 | 12 | Reception infrastructure; international cooperation; just-transition for receiving regions | 8 | Migration, social-affairs | Open |
| REG-024 | Inter-cell mobility constrained by informal barriers | CUL-I2 risk | 2 | 3 | 6 | Ombuds reporting; constitutional protection of movement; anti-discrimination enforcement | 4 | Ombuds, courts | Open |
| REG-025 | Restorative-justice quality dilutes at scale | ASM-013 | 3 | 3 | 9 | Program-design standards; outcome auditing; victim consent | 6 | Justice | Open |
| REG-026 | Reform-fatigue collapses adoption coalition | ASM-038 | 3 | 4 | 12 | Sequenced reform; visible early wins; coalition maintenance; just-transition | 8 | Adoption-team leadership | Open |
| REG-027 | International cooperation insufficient for tax / AI / climate / biosecurity | ASM-020 | 4 | 4 | 16 | Diplomatic priority; coalition-of-the-willing; unilateral measures where feasible | 12 | Foreign-affairs | Open |
| REG-028 | Decision-log volume collapses into boilerplate | ASM-022 | 3 | 2 | 6 | Audit of log quality; sampling and external review; reasoning standards | 4 | Audit office, adversarial-review | Open |
| REG-029 | Encryption-vs-investigation friction becomes politically unsustainable | DEC-016 | 2 | 3 | 6 | Targeted-access infrastructure; investigative-capacity investment; transparency on case outcomes | 4 | Justice, cyber-agency | Open |
| REG-030 | Indigenous and customary law conflict with universal rights produces durable strife | CON-020 | 2 | 3 | 6 | Participatory accommodation; courts; reparative resources | 4 | Justice, ombuds | Open |
| REG-031 | AI safety regulator captured | RSK-001, RSK-010 | 2 | 5 | 10 | Independence protections; adversarial-review; international peer pressure | 6 | TAI-A1, GOV-B5 | Open |
| REG-032 | Reserve programs atrophy in peacetime | ASM-032 | 3 | 3 | 9 | Drill schedules; audit requirements; budget protection | 6 | Defense, infrastructure | Open |
| REG-033 | Educational mobility does not improve despite funding equalization | RSK-028, ASM-016 | 3 | 4 | 12 | Curriculum + teacher reform alongside funding; equity tracking; targeted supports | 8 | Education | Open |
| REG-034 | Pay-ratio cap induces firm fragmentation defeating intent | ASM-003 | 3 | 2 | 6 | Anti-fragmentation rules; sectoral wage boards; review and adjustment | 4 | Economy, antitrust | Open |
| REG-035 | Tertiary education quality collapses under low-cost regime | ASM-015 | 2 | 3 | 6 | Quality standards; research funding; institutional autonomy with public-mission accountability | 4 | Higher education | Open |
| REG-036 | Geoengineering deployment outside framework | RSK-041 | 2 | 5 | 10 | International governance work; explicit prohibition on unilateral deployment | 7 | Foreign affairs, science | Open |
| REG-037 | Pluralism erodes through mass-cultural drift | RSK-017 | 2 | 3 | 6 | Constitutional protection; minority-cultural support; pluralist civic infrastructure | 5 | Community-cultural ministries | Open |
| REG-038 | Sentence-length growth despite reform | RSK-019 | 2 | 3 | 6 | Constitutional cap; proportionality review; audit | 4 | Justice | Open |
| REG-039 | Public-service workforce shortage persists | ASM-029 | 3 | 3 | 9 | Pay competitiveness; conditions; status investment | 6 | Civil-service commission | Open |
| REG-040 | Cap-and-dividend ecological scheme captured into rent | ECN-B3 | 2 | 3 | 6 | Auction design; revenue transparency; per-citizen dividend mechanism | 4 | Ecology regulator | Open |
| REG-041 | Long-horizon impact statements become ceremonial | ASM-034 | 3 | 2 | 6 | Future-generations advocate enforcement; statement-quality audit | 4 | GOV-B7 | Open |
| REG-042 | Beneficial-ownership transparency under-implemented | LAW-AC | 3 | 3 | 9 | Anti-corruption commission; international cooperation; registry audits | 6 | Anti-corruption commission | Open |
| REG-043 | Civilian-control multi-modal first-response model leaves responders unsafe | ASM-023 | 2 | 3 | 6 | Risk-assessment in dispatch; police-backed escalation; responder training | 4 | Public-safety service | Open |
| REG-044 | Universal-floor inflation indexing destabilizes wage-price expectations | ASM-021 area | 2 | 3 | 6 | Macroprudential coordination; supply-side response; transparent rules | 5 | Central bank | Open |
| REG-045 | Anti-pluralist movement uses constitutional protections to consolidate | TZ-002 | 2 | 5 | 10 | Constitutional courts; non-derogable rights; civil-society capacity | 7 | All institutions | Open |
| REG-046 | Aggregated-data release allows re-identification | TAI-D10 | 2 | 3 | 6 | De-identification standards; re-identification criminal liability; risk-assessment | 4 | Data-protection authority | Open |
| REG-047 | Land-value tax assessment captured by incumbent land owners | ASM-005 | 3 | 3 | 9 | Independent assessment; transparent methodology; periodic review | 6 | Treasury, ombuds | Open |
| REG-048 | Multi-jurisdictional reform-momentum fractures | ASM-010 | 3 | 4 | 12 | Coalition discipline; phased reforms; legitimacy investments | 9 | Reform leadership | Open |

## Top Risks by Composite

After mitigation (residual):

1. REG-008 AI capability outpaces governance (residual 12)
2. REG-027 International cooperation insufficient (residual 12)
3. REG-019 Mental-health workforce shortage (residual 11)
4. REG-001 Adversarial-review body captured / starved (residual 10)
5. REG-006 Ecological caps breached (residual 10)
6. REG-009 Election integrity compromised (residual 10)
7. REG-007 Cyber attack cascade (residual 9)
8. REG-011 Pandemic exceeds capacity (residual 9)
9. REG-026 Reform fatigue collapses coalition (residual 8)
10. REG-013 Despair-meaning crisis deepens (residual 9)

## Risk Management Discipline

- Quarterly review of risk register by adversarial-review body.
- Risks with residual ≥ 10 reviewed monthly.
- New risks added by future iterations get next available ID.
- Closed risks remain in register with closure rationale.
- Owners required to publish quarterly status.

## Cross-References

- ART-006 failure-mode register: source of many risks.
- ART-021 stress-test scenarios: tests for risk dynamics.
- ART-027 decision log: decisions that affect risk profile.
- ART-028 assumption register: assumptions whose failure generates risks.
- ART-031 adversarial review: qualitative critique of mitigations.
