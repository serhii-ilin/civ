# Decision Log

Artifact ID: ART-027
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: all

## Purpose

Record the major design decisions made in this iteration with rationale, alternatives considered, evidence cited, and conditions that would trigger re-visit. Decisions are recorded chronologically; cross-references to architecture and review artifacts identify where the decision is implemented or might be challenged.

The decision log is a memory device. It does not by itself settle disputes; future iterations may revise any decision under the iteration protocol.

## Format

```text
DEC-XXX | Date | Scope (module/artifact ID) | Decision | Alternatives | Rationale | Evidence | Revisit Trigger
```

## Decisions

### DEC-001 | 2026-05-27 | ART-008 / VAL-019 | Adopt "internal observability with secure boundaries" as a core value

- Decision: VAL-019 makes institutional observability and external-boundary discipline a constitutional value, separate from but related to privacy (VAL-015), transparency (within VAL-019), and self-correction (VAL-018).
- Alternatives: (a) treat observability as a procedural rule under VAL-018 self-correction; (b) collapse observability into VAL-015 privacy.
- Rationale: observability is structurally different from self-correction (it is the mechanism that enables correction); collapsing into privacy obscures the distinction between transparency for institutions and protection for persons. A dedicated value sets up the tradeoff zones (TZ-004, TZ-009) cleanly.
- Evidence: CLM-090 procedural fairness; CLM-189 measurement distortion warning; RSK-009 surveillance risk; RSK-034 observability creep.
- Revisit trigger: SCN-014 (observability-creep) results showing that the separate value is not load-bearing, or that it creates surveillance backdoor.

### DEC-002 | 2026-05-27 | ART-009 / GOV-B1, GOV-B6 | Use both citizens' assembly and sortition chamber, not just one

- Decision: a sortition body (GOV-B1) is established for deliberative work, and a parallel sortition chamber (GOV-B6) plays specific constitutional roles (confirmation, referenda).
- Alternatives: (a) single sortition body covering both functions; (b) no sortition body, rely on elected and judicial bodies only.
- Rationale: separation reduces capture risk and allows different procedures (long deliberation vs. confirmatory vote) without overloading a single body.
- Evidence: CLM-018 sortition durability is contested; CLM-101, CLM-102 mixed evidence on deliberative bodies.
- Revisit trigger: SCN-019 (sortition durability) showing one body type fails reliably; or evidence that two bodies produce conflicting legitimacy claims.

### DEC-003 | 2026-05-27 | ART-009 / GOV-B5 | Establish standing Adversarial Review Body

- Decision: a permanent body with subpoena and publication power and mandate to disagree with consensus is created.
- Alternatives: (a) ad hoc oversight commissions; (b) rely on judicial review and legislative oversight only.
- Rationale: standing adversarial review is one of the framework's load-bearing capture defenses; failure modes RSK-001, RSK-003, RSK-019, RSK-022, RSK-023 all weaken without it.
- Evidence: CLM-015, CLM-016 democratic-backsliding patterns; CLM-189 measurement distortion needs adversarial check.
- Revisit trigger: GOV-B5 itself becomes captured or sclerotic; or simulation shows accountability holds without it.

### DEC-004 | 2026-05-27 | ART-010 / ECO-L1-L5 | Five-layer mixed economy

- Decision: economy is divided into commons, public provisioning, regulated market, discretionary market, and structurally separate regimes (land, finance, ecological commons).
- Alternatives: (a) market by default with public goods at margins; (b) public sector by default with markets at margins; (c) three-layer (commons / public / market).
- Rationale: distinct layers permit different governance suited to different goods; separate land and finance regimes acknowledge their structurally different dynamics. Three-layer collapses critical distinctions.
- Evidence: CLM-006, CLM-010, CLM-020-021, CLM-024, CLM-070, CLM-080.
- Revisit trigger: SCN-016, SCN-017 simulations showing layer boundaries collapse under stress; or evidence that one or more layers is unnecessary.

### DEC-005 | 2026-05-27 | ART-010 / ECO-I1 | Universal floor (cash) on top of universal services

- Decision: a cash floor is provided in addition to commons (L1) and universal services (L2), not as a substitute for them.
- Alternatives: (a) cash-only universal basic income with private purchase of services; (b) services-only without cash floor; (c) negative income tax.
- Rationale: pure cash is regressive vis-a-vis market power; pure services constrains autonomy; combination addresses both. Behavioral evidence (B-016) supports relieving material scarcity before expecting civic capacity.
- Evidence: CLM-025, CLM-026, CLM-040.
- Revisit trigger: SCN-016 showing cash-floor real value erodes under inflation while services hold; or evidence that combination is fiscally unsustainable.

### DEC-006 | 2026-05-27 | ART-010 / ECO-I2 | Pay-ratio caps within firms

- Decision: firm-level pay-ratio cap (default 20:1; tighter for L1/L2 firms).
- Alternatives: (a) no cap; (b) sectoral wage councils only; (c) confiscatory top-rate tax instead of ratio.
- Rationale: structural moderation of inequality is more durable than tax alone (CLM-021); ratio is enforceable within firms.
- Evidence: BMK-020 Mondragon pay-ratio drift case; CLM-020-022.
- Revisit trigger: evidence that ratio induces firm fragmentation or relocation that defeats the purpose; revisit ratio level after 5 years of data.

### DEC-007 | 2026-05-27 | ART-011 / LAW-CJ3 | Restorative justice as primary alternative for eligible offenses

- Decision: restorative pathways are the default alternative for eligible offenses where victim, offender, and community consent.
- Alternatives: (a) retributive default with restorative as exception; (b) full restorative for non-violent offenses by statute.
- Rationale: restorative outcomes are better on average for many offenses but variable by program design (CLM-091). Choice between primary and exceptional alternative affects scale.
- Evidence: CLM-091, SRC-048, SRC-049, SRC-101.
- Revisit trigger: 10-year outcome data; if restorative programs systematically underserve victims, revisit.

### DEC-008 | 2026-05-27 | ART-011 / LAW-P2 | Multi-modal public-safety service

- Decision: non-violent calls go to civilian first responders (mental-health teams, social workers, mediators); armed police only for violent incidents.
- Alternatives: (a) sworn-officer first response default; (b) civilian-only for all calls.
- Rationale: matches B-009 trauma awareness and reduces use-of-force-related harm; benchmark of multi-modal models in some jurisdictions showed improvement.
- Evidence: CLM-192, RSK-019.
- Revisit trigger: evidence that civilian responders are over-exposed to violence; revisit risk-assessment in dispatch.

### DEC-009 | 2026-05-27 | ART-012 / HEA-A1 | Universal coverage with single public payer

- Decision: single public payer at national tier with regional administration; provider mix plural.
- Alternatives: (a) multi-payer regulated insurance; (b) fully public delivery; (c) means-tested coverage.
- Rationale: single-payer captures administrative efficiency and bargaining power while plural provision avoids monopoly delivery risks. Means-tested approaches consistently produce gaps and stigma.
- Evidence: BMK-030 universal-coverage cases.
- Revisit trigger: SCN-006 pandemic scenarios showing payer model under-performs; or fiscal sustainability strains.

### DEC-010 | 2026-05-27 | ART-013 / EDU-E1 | Equalized school funding across regions

- Decision: school funding equalized across regions and within regions, with need-weighting.
- Alternatives: (a) locally-funded (property tax) default; (b) flat per-student.
- Rationale: locally funded school finance is a known channel of class reproduction (CLM-110, RSK-028); need-weighted is consistent with capability-equity goals.
- Evidence: CLM-052, CLM-110.
- Revisit trigger: outcome data shows funding equalization without curriculum and teacher reform did not close gaps; deepen reform.

### DEC-011 | 2026-05-27 | ART-013 / EDU-E7 | Defer tracking to upper secondary

- Decision: pathway tracking is deferred to roughly age 16; common curriculum until then.
- Alternatives: (a) early tracking; (b) no tracking at any age.
- Rationale: early tracking reproduces class structure; full untracking can sacrifice depth. Deferred-tracking compromise.
- Evidence: cross-country PISA pattern; CLM-110.
- Revisit trigger: evidence of insufficient depth for academic-track students; revisit pathway design.

### DEC-012 | 2026-05-27 | ART-014 / CUL-C1 | Cell scale 5,000-15,000

- Decision: working scale for community cells is in the range 5,000-15,000 members.
- Alternatives: smaller (under 1,000) or larger (over 50,000).
- Rationale: lower bound is institutional sufficiency (services and governance); upper bound is relational legibility consistent with Dunbar layering and B-007.
- Evidence: CLM-062, B-007.
- Revisit trigger: pilot data showing the band produces dysfunction at one end; recalibrate.

### DEC-013 | 2026-05-27 | ART-015 / ECN-B1 | Hard ecological caps in constitution

- Decision: GHG budget, watershed water budgets, biodiversity floors, soil-quality floors, pollution caps are constitutionally binding.
- Alternatives: (a) statutory only; (b) target-based without hard cap.
- Rationale: constitutional ceiling prevents political-economy default to cap-breaching; future-generations advocate alone insufficient.
- Evidence: CLM-027, CLM-070, CLM-072, RSK-006, RSK-016.
- Revisit trigger: caps held in simulation only because of unrealistic policy compliance; if real-polity adoption shows non-compliance norm, revise enforcement design.

### DEC-014 | 2026-05-27 | ART-015 / ECN-L1 | Land cannot be unconditionally owned

- Decision: land tenure mixes private (with land-value tax), public, community-trust, indigenous, common; no unconditional fee-simple capture of community-generated value.
- Alternatives: (a) full private property; (b) full public ownership.
- Rationale: full private property generates speculation, capture, and intergenerational inequality (CLM-110, RSK-025); full public ownership has its own failure modes (BMK-012 lessons). Mixed system with land-value tax addresses both.
- Evidence: CLM-110, BMK-008, BMK-020.
- Revisit trigger: implementation challenges in adoption polities show land-value-tax administration not feasible at scale; revisit instrument.

### DEC-015 | 2026-05-27 | ART-016 / TAI-R2 | Specific AI prohibitions in Tier 1

- Decision: enumerated prohibitions include social credit scoring, mass biometric identification in public, manipulative AI exploiting vulnerable groups, autonomous lethal-decision systems, AI-enabled CSAM.
- Alternatives: (a) general principles only; (b) longer or shorter prohibition list.
- Rationale: structural prohibition is more enforceable than principle; the listed items are sufficiently dangerous that exceptions create unmanageable risk.
- Evidence: CLM-081, CLM-082, RSK-009, RSK-010, RSK-042.
- Revisit trigger: technology trajectory shifts; prohibitions become irrelevant or create avoidance dynamics that move risks elsewhere.

### DEC-016 | 2026-05-27 | ART-016 / TAI-S6 | No encryption back-doors

- Decision: strong encryption supported; lawful access through targeted, judicially authorized means; no general back-doors.
- Alternatives: (a) lawful-access back-doors; (b) ban on strong encryption.
- Rationale: back-doors are exploited by adversaries; lawful access is achievable through targeted action.
- Evidence: cryptography research consensus; CLM-085 cyber-risk evidence.
- Revisit trigger: investigative impossibility for serious crime makes the rule unsustainable; revisit specific authorized-access mechanisms with strong oversight.

### DEC-017 | 2026-05-27 | ART-017 / DEF-M6 | Prohibit autonomous lethal decisions

- Decision: framework prohibits autonomous lethal-decision systems where humans are not in meaningful command.
- Alternatives: (a) allow with safeguards; (b) prohibit even human-in-the-loop systems in certain contexts.
- Rationale: meaningful human control is the only currently defensible standard for lethal force; safeguards in autonomous-decision systems are unproven at the relevant capability level.
- Evidence: international debates around autonomous-weapons systems; CLM-084.
- Revisit trigger: international consensus shifts; or technology trajectory shifts.

### DEC-018 | 2026-05-27 | ART-009 / GOV-D5 | Emergency-powers default expiry 30 days; cumulative cap 180 days without supermajority

- Decision: emergency powers default to 30-day expiry; cumulative without supermajority capped at 180 days.
- Alternatives: shorter or longer; no cumulative cap; supermajority for any extension.
- Rationale: short default forces frequent legitimization; cumulative cap prevents ratchet (RSK-035, SCN-012).
- Evidence: BMK-013 Weimar Article 48 lesson; many democratic-backsliding cases.
- Revisit trigger: emergencies in real adoption polities require longer; revisit balance with explicit reasoning.

### DEC-019 | 2026-05-27 | ART-017 / DEF-MIG2-4 | Plural migration pathways with accessible naturalization

- Decision: lawful immigration pathways include family, work, study, humanitarian, with accessible naturalization after qualifying residency.
- Alternatives: (a) restrictive immigration with rare naturalization; (b) open borders with looser naturalization.
- Rationale: balanced approach respects rights, integration capacity, and demographic resilience.
- Evidence: BMK-005 Nordic experience; CLM-110, RSK-012, RSK-013.
- Revisit trigger: climate-migration scale exceeds reception capacity (SCN-005); revisit reception infrastructure.

### DEC-020 | 2026-05-27 | ART-018 / TAR-P5 | Cryptographic separation of public-observability and personal-data systems

- Decision: technical infrastructure cryptographically separates institutional observability from personal-data systems.
- Alternatives: (a) policy-only separation; (b) integrated systems with access controls.
- Rationale: policy-only separation has repeatedly failed to prevent surveillance creep (RSK-034); cryptographic separation is harder to bypass undetected.
- Evidence: many surveillance-creep cases; CLM-080.
- Revisit trigger: cryptographic standards advance to permit homomorphic or zero-knowledge alternatives; revisit specific implementation.

### DEC-021 | 2026-05-27 | ART-024 / Adoption sequencing | Protect first, redistribute second

- Decision: foundational protections (rights, observability, adversarial review, independent regulators) precede expanded redistribution and regulation.
- Alternatives: (a) all reforms in parallel; (b) redistribute first to build legitimacy.
- Rationale: redistribution programs depend on functioning anti-capture institutions; reversing the order risks capture of the redistribution programs themselves.
- Evidence: democratic-backsliding pattern of capturing institutions first; CLM-015, CLM-016.
- Revisit trigger: real adoption polity shows that public legitimacy requires early visible redistribution; revisit sequencing per context.

### DEC-022 | 2026-05-27 | All | Goodhart-aware indicator design

- Decision: no single indicator drives a budgetary or staffing decision; multi-indicator panels with regular auditing for gaming.
- Alternatives: high-stakes single-indicator regimes (common in many real systems).
- Rationale: single-indicator regimes systematically distort behavior (CLM-189); multi-indicator with auditing reduces but does not eliminate distortion.
- Evidence: SRC-071, SRC-072.
- Revisit trigger: indicator-design audit shows reliable gaming despite multi-indicator approach; revisit specific indicators.

### DEC-023 | 2026-05-27 | All | Decision documentation discipline

- Decision: all framework architecture decisions are recorded in this log with rationale; all major implementation decisions in the adopting polity follow analogous discipline.
- Alternatives: ad-hoc documentation; oral tradition.
- Rationale: enabling future revision requires the original rationale.
- Evidence: institutional-memory failure mode (RSK-031).
- Revisit trigger: decision-log discipline itself fails (volume too high, rationale boilerplate).

## Open Decision Areas (Pending Future Iterations)

- DEC-OPEN-001: exact sortition compensation level (ART-009, GOV-B1).
- DEC-OPEN-002: specific wealth-tax thresholds calibrated to polity (ART-010, ECO-T2).
- DEC-OPEN-003: nuclear-energy role in transition mix (ART-015, ECN-E2).
- DEC-OPEN-004: party-law specifications (ART-009).
- DEC-OPEN-005: relationship with non-human persons (ART-008 Article VII).
- DEC-OPEN-006: geoengineering governance specifics (ART-015, RSK-041).
- DEC-OPEN-007: foundation-model AI capability thresholds (ART-016, TAI-R6).
- DEC-OPEN-008: emergency-power thresholds calibrated to climate-disaster-prone regions (ART-009, GOV-D5).

These decisions await further analysis, evidence, deliberation, or simulation, and are flagged for future iteration attention.
