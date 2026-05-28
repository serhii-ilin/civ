# Technology and AI Governance

Artifact ID: ART-016
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: MOD-TAI
Depends on: ART-008, ART-009, ART-011

## Purpose

Specify governance of digital technology, artificial intelligence, data, cybersecurity, observability infrastructure, automation transition, biosecurity, and dual-use research. Bound by `value-constitution.md` (ART-008), `governance-system.md` (ART-009), and `law-and-justice-system.md` (ART-011).

Core principles: (i) technology serves the value constitution, not the reverse; (ii) high-impact algorithmic systems are accountable, auditable, and contestable; (iii) data rights belong to people; (iv) institutional observability does not become surveillance of people; (v) critical digital infrastructure is treated as critical infrastructure.

## Architecture (TAI-A)

### TAI-A1 Independent AI Safety Regulator

- One of GOV-B10 regulators.
- Authority over: risk classification of AI systems, mandatory audits, incident reporting, conformity assessment, market-entry approval for high-risk systems, market surveillance.
- Powers: information requests, subpoena, fines, market-withdrawal orders, criminal referrals.
- Independence: protected funding; mixed-body appointment; published reasoning.

### TAI-A2 Data Protection Authority

- One of GOV-B10 regulators.
- Authority over data-rights enforcement (LAW-R4, VAL-015).
- Powers: investigate, audit, sanction, mandate corrective action.

### TAI-A3 Cybersecurity Agency

- National cybersecurity coordination; standards-setting; incident response; threat-intelligence sharing.
- Independent of intelligence services for civilian-facing mandates.

### TAI-A4 Public-Interest Technology Office

- Within GOV-B4; ensures public services have in-house tech capability; reduces dependence on private vendors for core public functions.
- Coordinates open-standards and open-source policies.

### TAI-A5 Standards Bodies

- National standards body with participation in international standards processes.
- Open and inclusive standards-setting; transparent voting.

## Data Rights and Privacy (TAI-D)

### TAI-D1 Constitutional Floor

- Personal data is protected by VAL-015 and LAW-R1.
- Members have rights to access, rectification, deletion, portability, object to processing, restrict processing.

### TAI-D2 Lawful Bases

- Personal data processing requires a lawful basis: consent (free, informed, specific, revocable), contractual necessity, legal obligation, vital interest, public-interest task, or carefully-balanced legitimate interest with transparent reasoning.
- Consent is not free in significant power asymmetries; cannot be tied to access where unrelated.

### TAI-D3 Purpose Limitation

- Data collected for one purpose cannot be reused for incompatible purposes without renewed lawful basis.
- Purpose specification required at collection.

### TAI-D4 Data Minimization

- Only data necessary for the specified purpose.
- Retention limits set in law and policy; defaults short.

### TAI-D5 Sensitive Data

- Health, genetic, biometric, religion, ethnicity, sexuality, political belief, trade-union membership data: elevated protection.
- Processing only with explicit consent or narrow statutory authority.

### TAI-D6 Children's Data

- Heightened protection; no behavioral advertising to children; strict consent regime for processing children's data.

### TAI-D7 Algorithmic Decision-Making

- Right to explanation for decisions with significant effect on rights or material outcomes.
- Right to human review.
- Prohibition on solely automated decisions in high-stakes domains (employment, credit, housing, education, criminal justice, public benefits) without specific safeguards.

### TAI-D8 Member Access to Own Data

- Subject-access requests fulfilled within set timeframes.
- Member-controlled personal-data wallet infrastructure available as public option.

### TAI-D9 Data Localization and Sovereignty

- Critical and sensitive data hosted under polity jurisdiction.
- Cross-border transfers permitted to jurisdictions with adequate protections; otherwise contractual and technical safeguards required.

### TAI-D10 De-Identification and Re-Identification

- De-identification standards set by TAI-A2.
- Re-identification attempts are criminal (HEA-D2 parallel).
- Aggregated data may be released for research and accountability under risk-assessed conditions.

### TAI-D11 Member Observability of Personal Data Use

- Each member can see logs of access to their data by public bodies (with delay for active investigations).
- Each member can see what categories of data are held about them by major private holders.

## AI Risk Classification (TAI-R)

### TAI-R1 Risk Tiers

The framework adopts a four-tier risk classification adapted from emerging international practice (CLM-083, SRC-079):

- Tier 1 — Unacceptable: prohibited.
- Tier 2 — High: market-entry approval, mandatory audit, ongoing surveillance.
- Tier 3 — Limited: transparency obligations, voluntary or sectoral standards.
- Tier 4 — Minimal: light-touch.

### TAI-R2 Tier 1 — Prohibited

- Social-credit-scoring of natural persons by state or commercial actors with cross-domain consequences.
- Mass biometric identification of natural persons in publicly accessible spaces in real time (with narrow exceptions: imminent severe threat, judicial authorization, time-limited, reported).
- Emotion-recognition in workplace and education for evaluative purposes.
- Manipulative AI techniques exploiting vulnerabilities of children, disabled persons, or other vulnerable groups.
- Predictive-policing systems based on profiling of natural persons without specific criminal-investigation justification.
- AI-enabled production of child sexual abuse material.
- Autonomous lethal-decision systems where humans are not in meaningful command of force decisions.
- Inferential systems that infer protected characteristics (ethnicity, religion, sexuality, political belief, health status) without specific consent for narrow purposes.

### TAI-R3 Tier 2 — High Risk

- Public-administration decisions affecting rights or material interests.
- Healthcare diagnosis and treatment-decision support.
- Criminal-justice risk assessment.
- Critical-infrastructure operations.
- Employment, education, credit, housing, and benefits decisions.
- Border, migration, and asylum systems.
- Election-related systems.
- Conformity assessment required before market entry; ongoing monitoring; human oversight required.

### TAI-R4 Tier 3 — Limited Risk

- Generative AI for content creation (with watermarking for synthetic media; disclosure of AI-content provenance).
- Chatbots interacting with members (disclosure of non-human counterparty required).
- Emotion-recognition outside Tier 1 contexts (consent and notice required).

### TAI-R5 Tier 4 — Minimal Risk

- General-purpose computational tools, recommendation systems on non-essential platforms, video games, productivity tools.
- Lighter obligations; voluntary standards encouraged.

### TAI-R6 General-Purpose AI Foundation Models

- Foundation models with broad capabilities subject to particular obligations: documentation, transparency on training data within reason, evaluation, red-teaming for misuse, computation and capability thresholds may trigger heightened obligations.
- Cross-border coordination required because models cross borders.

### TAI-R7 Open vs. Closed Models

- Open-weight models with public benefit are permitted; misuse mitigated through downstream regulation rather than upstream prohibition where feasible.
- Highly capable open models above defined thresholds may trigger pre-release safety review.

## Algorithmic Accountability (TAI-AC)

### TAI-AC1 Documentation

- Tier 2 systems require comprehensive documentation: purpose, training data, evaluation, known limitations, intended use, contraindications.
- Documentation accessible to regulators and to affected members in suitable form.

### TAI-AC2 Audit

- Independent audits for Tier 2 systems before deployment and periodically thereafter.
- Audit covers: accuracy, bias, robustness, security, alignment with purpose, conformity with rights protections.
- Audit findings public in summary form.

### TAI-AC3 Impact Assessment

- Algorithmic impact assessments for public-sector deployment of Tier 2 and Tier 3 systems.
- Public consultation required before deployment.

### TAI-AC4 Incident Reporting

- Mandatory reporting of significant incidents (rights violations, accuracy failures, security breaches).
- Reports anonymized as appropriate; aggregated reports public.

### TAI-AC5 Procurement Standards

- Public-sector procurement requires conformity with TAI standards.
- Contractors must allow audit, accept liability, and respect data-rights frameworks.

### TAI-AC6 Accountability Vesting

- Legal accountability for AI-system outcomes vested in identified humans: deployer, operator, or provider depending on configuration.
- "The algorithm decided" is not a legal defense.

### TAI-AC7 Right to Recourse

- Affected members can challenge automated decisions, request human review, request explanation, and seek judicial remedy.

## Member Observability Infrastructure (TAI-O)

The framework's commitment to internal observability (VAL-019) requires technical infrastructure. This section specifies that infrastructure.

### TAI-O1 Public Decision Logs

- A national decision-log infrastructure where every public body publishes machine- and human-readable records of decisions (GOV-O1).
- Standards-based; interoperable; archived permanently with redundancy.

### TAI-O2 Institutional Metrics Dashboards

- Public dashboards (GOV-O2) at national, regional, and local levels.
- Open API for civic and research use.
- Accessibility standards.

### TAI-O3 Audit Trails

- Internal audit trails for all data access by public-sector systems.
- Tamper-evident logging (e.g., cryptographically chained).
- Independent oversight access (GOV-B5, GOV-B8).
- Members can see access logs for their own data.

### TAI-O4 Algorithmic Registries

- Public registry of algorithmic systems used by public bodies, with risk classification, documentation, audit status, contact for recourse.

### TAI-O5 Lobbying and Influence Logs

- GOV-A3 (lobbying transparency) operationalized through standard data schema and a public registry.

### TAI-O6 Cryptographic Separation

- Personal-data systems cryptographically isolated from public-observability systems.
- Aggregated reports use differential-privacy or secure-multiparty techniques where individual privacy is at risk.

### TAI-O7 Limits

- Personal data is not made public for observability.
- Access controls on whistleblower identities, vulnerable-population data, ongoing-investigation data.
- Observability creep (RSK-034) audited annually.

## Cybersecurity (TAI-S)

### TAI-S1 Baseline Standards

- All public-sector systems meet a defined baseline (modeled on NIST CSF / EU NIS2 family).
- Critical-infrastructure operators (public and regulated private) meet elevated standards.

### TAI-S2 Vulnerability Disclosure

- Coordinated vulnerability-disclosure framework.
- Bug-bounty programs encouraged.
- "Hacking back" prohibited.

### TAI-S3 Incident Response

- National CSIRT coordinating with sectoral teams.
- Mandatory reporting of significant incidents.
- Mutual-aid agreements internationally.

### TAI-S4 Critical-Infrastructure Cyber

- Air-gapping or strong segmentation for operational technology of critical-infrastructure systems.
- Continuous monitoring; rehearsed response.
- See RSK-008.

### TAI-S5 Supply-Chain Security

- SBOM (Software Bill of Materials) for public-sector procurement.
- Cryptographic-supply-chain integrity controls.

### TAI-S6 Encryption

- Strong encryption supported; member access to encryption protected.
- Lawful-access frameworks limited to targeted, judicially authorized actions; no general back-doors.

### TAI-S7 Workforce

- Public-sector cyber-talent strategy.
- Public-interest training programs.

## Digital Identity (TAI-ID)

### TAI-ID1 Decentralized Identity

- Public-option digital identity with strong privacy.
- Members can prove attributes (age, residency, qualifications) without revealing identity itself.
- Verifiable credentials standards.

### TAI-ID2 Anti-Exclusion Safeguards

- Non-digital fallbacks available for every service.
- Access support for digitally excluded members.

### TAI-ID3 Account Recovery and Continuity

- Recovery mechanisms that do not require single trusted intermediary.
- Account-deletion right.

## Public-Sector Digital (TAI-PS)

### TAI-PS1 Open Standards by Default

- Public-sector systems use open standards; vendor lock-in avoided.

### TAI-PS2 Open-Source by Default

- Publicly developed code is open-source unless specific security or contractual reasons require otherwise.

### TAI-PS3 In-House Capacity

- TAI-A4 ensures sufficient in-house capability that public services are not held hostage by vendors.

### TAI-PS4 Procurement

- Procurement criteria include open standards, security, accessibility, sustainability, data-rights compliance, exit-friendliness.

## Automation Transition (TAI-AT)

### TAI-AT1 Tax and Transfer

- ECO-T5 automation tax funds transition.
- Universal floor (ECO-I1) provides security across transition.

### TAI-AT2 Workforce Transition

- Reskilling entitlements (EDU-R).
- Sectoral transition plans.
- Just-transition principles applied.

### TAI-AT3 Quality of Work

- Automation deployed to reduce harmful work; productivity gains shared with workers.
- Worker voice in deployment decisions (ECO-W2).

### TAI-AT4 Hours Reduction

- Productivity gains may be taken as reduced working time, not only as higher consumption.

### TAI-AT5 Public-Sector Discipline

- Public services automated to improve access and quality, not to reduce dignity of work for clients or staff.

## Biosecurity and Dual-Use Research (TAI-B)

### TAI-B1 Biosafety Standards

- Laboratory biosafety standards aligned with international best practice.
- Inspection regime.
- Mandatory incident reporting.

### TAI-B2 Dual-Use Research Oversight

- Institutional review for research with significant misuse potential.
- Publication restrictions only with narrow justification and procedural review.

### TAI-B3 Gain-of-Function Research

- Subject to strict oversight; international coordination prioritized.

### TAI-B4 Synthetic Biology

- DNA-synthesis-provider screening requirements.
- Engineered-organism release restrictions.
- Public dialogue and consent for major decisions.

### TAI-B5 Surveillance and Privacy

- Biosecurity surveillance limited to public-health purposes (HEA-P1).
- No fusion with criminal-investigation systems without judicial process.

## International Cooperation (TAI-IC)

- Active participation in standards bodies, treaty negotiations, joint research.
- Particular priority on: AI safety governance, biosecurity, cybersecurity, cross-border data flows, dual-use technology, climate-related technology.

## Open Issues

- Foundation-model regulation (TAI-R6) is fast-evolving; thresholds must adapt with capability and deployment patterns.
- Open vs. closed models (TAI-R7) policy is contested; the framework keeps a permissive default with downstream regulation, but high-capability open models may need pre-release review.
- Encryption-vs-law-enforcement balance (TAI-S6) is politically contested; the framework leans strongly against back-doors, accepting some investigative friction.
- Algorithmic-decision prohibition in high-stakes domains (TAI-D7) sets a high bar; some efficiency lost; the tradeoff is accepted to protect rights.
- Biosecurity governance (TAI-B) cannot be solved unilaterally; framework relies on international coordination.
- Member observability infrastructure (TAI-O) is a large public-investment program; transition path required (ART-024).
- Open-source-by-default in public sector (TAI-PS2) faces vendor and procurement-culture resistance; transition managed in ART-026.

## Cross-References

- Bound by: VAL-001, VAL-006, VAL-009, VAL-015, VAL-018, VAL-019.
- Coordinates with: ART-009 (governance), ART-011 (law), ART-010 (economy), ART-013 (education), ART-015 (infrastructure), ART-017 (defense, including cyber and bio), ART-024 (implementation).
- Tested in: cyber-attack scenarios, AI-information-shock scenarios, observability-creep scenarios.
