# Technical Architecture

Artifact ID: ART-018
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: all architecture modules
Depends on: ART-008 through ART-017

## Purpose

Integrate the architecture modules (ART-008 through ART-017) into a coherent technical specification. Define common interfaces, data flows, dependencies between subsystems, shared standards, and cross-cutting patterns. Provides the spec against which the simulation (ART-019) and implementation (ART-024) are built.

This artifact does not restate each module; it specifies how they connect.

## System Model

The framework is modeled as a multi-tier institutional system composed of nine interacting subsystems plus a constitutional layer. Each subsystem has an owning module, interfaces to others, observable state, and accountability paths.

### Layers (TAR-L)

- L0 Constitutional: value constitution (ART-008), governance bodies (ART-009), legal framework (ART-011). The persistent rules-of-the-rules layer.
- L1 Public Goods and Commons: ecology and infrastructure (ART-015), health (ART-012), education (ART-013), commons layer of economy (ART-010).
- L2 Civic Architecture: community and culture (ART-014), participatory governance instruments (ART-009).
- L3 Production and Exchange: regulated and discretionary market layers (ART-010).
- L4 External Interfaces: defense, foreign relations, migration, boundary controls (ART-017).
- L5 Cross-Cutting Infrastructure: technology, AI, data, observability infrastructure (ART-016).
- L6 Self-Correction: adversarial review, audit, ombuds, simulation, decision and assumption logs (ART-009 GOV-B5 / B8 / B9, this iteration's review artifacts).

## Subsystem Interfaces

Each entry lists which subsystem provides a service, which consumes it, and the binding constraints.

### TAR-I1 Governance → All

- Provides: legal authority, decision-making bodies, dispute resolution, rule-changing procedure.
- Consumed by: every subsystem.
- Binding: ART-008 values; GOV-O observability; GOV-A capture defenses.

### TAR-I2 Law → All

- Provides: enforcement mechanisms, rights protections, procedural standards.
- Consumed by: every subsystem.
- Binding: ART-008 values; LAW-R rights; LAW-O transparency.

### TAR-I3 Economy → Health, Education, Community, Ecology, Defense

- Provides: financing, labor, allocation of resources beyond commons.
- Consumed by: subsystems that require funding and workforce.
- Binding: ECO-T (tax instruments), ECO-W (labor rights), ECO-L5 (structurally separate regimes).

### TAR-I4 Ecology / Infrastructure → All

- Provides: physical substrate, energy, water, food, transport, housing.
- Consumed by: every subsystem.
- Binding: ECN-B ceilings; ECN-IC continuity; ECN-A accounting.

### TAR-I5 Health → All

- Provides: population-health condition, mental-health infrastructure, public-health response.
- Consumed by: every subsystem (working-age workforce, school-age learners, civic participation).
- Binding: HEA-P (privacy in surveillance), HEA-D (data infrastructure).

### TAR-I6 Education → All

- Provides: civic competence, technical skills, labor force.
- Consumed by: every subsystem.
- Binding: EDU-C (curriculum), EDU-E (equity), EDU-G (governance).

### TAR-I7 Community / Culture → All

- Provides: cohesion, conflict resolution at low scale, care infrastructure, pluralism.
- Consumed by: every subsystem.
- Binding: CUL-P (pluralism), CUL-CR (conflict resolution), CUL-CA (care).

### TAR-I8 Technology / AI → All

- Provides: digital systems, observability infrastructure, automation, communication, data services.
- Consumed by: every subsystem.
- Binding: TAI-D (data rights), TAI-R (risk classification), TAI-O (observability discipline), TAI-S (cyber).

### TAR-I9 Defense / External → All

- Provides: external security, foreign relations, migration management, biosecurity, boundary integrity.
- Consumed by: every subsystem during stress; routinely by economic, biosecurity, and digital subsystems.
- Binding: DEF-C (crisis-power limits), DEF-B (boundary audit), DEF-MIG (rights for non-members).

## Cross-Cutting Patterns

### TAR-P1 Multi-Tier Subsidiarity

- Authority defaults to the lowest tier capable of effective action.
- Higher tiers intervene where: scale effects, rights protection, externality coordination, or local capture make local action insufficient.
- Conflicts resolved through the inter-tier processes specified in GOV-I.

### TAR-P2 Mixed Selection

- No single selection method (election, sortition, appointment, civil-service career) dominates.
- Each body uses a method matched to its function; combined methods for high-stakes appointments.
- Capture resistance comes from the mix, not from any single method.

### TAR-P3 Rotation and Renewal

- Every authority-bearing role has term limits, rotation cycles, or both.
- Institutional memory preserved through staggering and through career civil service (GOV-S4).

### TAR-P4 Multi-Method Accountability

- Every decision faces: judicial review (LAW-C), audit (GOV-B8), adversarial review (GOV-B5), ombuds (GOV-B9), public observability (TAI-O), member recall or removal where applicable (GOV-R).
- Failure of one channel does not collapse accountability.

### TAR-P5 Observable Public, Private Persons

- Institutional decisions, processes, and aggregated outcomes are observable.
- Personal data is private; flows are controlled and audited (TAI-D, VAL-019, VAL-015).
- Cryptographic separation enforced (TAI-O6).

### TAR-P6 Standing Adversarial Review

- A standing body (GOV-B5) is funded to disagree, audit, and publish.
- The body cannot be silenced or dissolved without constitutional amendment.
- Whistleblower protections feed into this body.

### TAR-P7 Long-Horizon Advocacy

- Future-generations advocate (GOV-B7) consulted on long-horizon decisions.
- Long-horizon impact statements required for major decisions.
- Constitutional ecological ceilings (ECN-B1) bind present-tense decisions to long-horizon constraints.

### TAR-P8 Crisis Discipline

- Emergency powers exist (GOV-D5, LAW-E, DEF-C) with hard limits.
- Non-derogable rights hold in crisis (LAW-R5).
- Sunset and review automatic.

### TAR-P9 Standards-Based Interoperability

- Public-sector systems use open standards (TAI-PS1).
- Cross-subsystem data flows are specified, audited, and minimized.

### TAR-P10 Goodhart-Aware Measurement

- No single metric drives a budget, hiring, or program decision.
- Indicators are reviewed regularly for gaming and distortion (CLM-189).

## Data Flows

The following flows define how information moves between subsystems. Each flow is specified by purpose, data minimization rule, and audit obligation.

### TAR-DF1 Personal Health Data → Health Providers

- Purpose: clinical care.
- Lawful basis: care relationship or consent.
- Sharing: only with member consent; audit trail.

### TAR-DF2 Public Health Surveillance Data

- Purpose: outbreak detection, population-health monitoring.
- Lawful basis: statutory authority for defined reportable conditions.
- Minimization: aggregate where possible; identifiable only with justification.
- Sharing with law enforcement: prohibited absent specific judicial process.

### TAR-DF3 Education Records

- Purpose: student support and credential issuance.
- Lawful basis: education relationship and consent.
- Sharing: limited; family receives child's records; aggregate research with de-identification.

### TAR-DF4 Tax and Financial Records

- Purpose: tax assessment and enforcement.
- Lawful basis: tax law.
- Sharing: limited inter-agency; cross-border sharing under treaty; member access to own records.

### TAR-DF5 Justice System Records

- Purpose: case management and public accountability.
- Public: case docket, judgments, aggregated statistics.
- Private: personal identifiers of victims, witnesses, minors, sealed records; access via court order.

### TAR-DF6 Civic Participation Records

- Purpose: enable voting, sortition selection, participatory budgeting.
- Aggregate participation public; individual records private.

### TAR-DF7 Institutional Decision Logs

- Purpose: member observability.
- Public by default; narrow closure under defined criteria.

### TAR-DF8 Audit Trails

- Purpose: integrity and accountability.
- Internal access by audit, ombuds, adversarial review.
- Aggregate findings public.

### TAR-DF9 Surveillance Data (Lawful)

- Purpose: targeted investigation or national security.
- Lawful basis: judicial warrant.
- Minimization, retention limits, post-investigation disclosure.

### TAR-DF10 Biosecurity and Cross-Border Health

- Purpose: prevent biological-agent outbreaks.
- Coordinated with international bodies; data minimization.

## Interfaces with Non-Members

The framework's interfaces with people who are not members of the polity (visitors, residents in process, asylum seekers, stateless persons, foreign nationals on home territory) must respect LAW-R5 non-derogable rights for all persons under jurisdiction and the specific protections in ART-017.

### TAR-NM1 Border Crossings

- Police-style process under rule of law; no military-style screening absent specific threat.
- Asylum process triggered automatically on protection claim.
- Detention only with specific authority; alternatives preferred.

### TAR-NM2 Residency

- Long-term residents have most rights of citizens; specific exclusions narrow (voting in national elections; specific public-office positions; military service).
- Path to naturalization clearly defined and accessible (DEF-MIG4).

### TAR-NM3 Visitors

- Standard rights against arbitrary detention, due process, freedom from torture, access to legal process.

### TAR-NM4 Stateless Persons

- Identification and pathway to status (DEF-MIG6).

## Risk Pathways and Mitigations

Drawn from `failure-mode-register.md`:

| Risk | Primary Subsystem | Secondary Subsystems | Architectural Mitigation |
| --- | --- | --- | --- |
| RSK-001 Elite capture | Governance | Economy, Justice | Mixed selection, transparency, sortition body, adversarial review |
| RSK-002 Demagogue ascent | Governance | Media, Justice | Multi-body checks, independent courts, public-service media, anti-incitement law within speech protection |
| RSK-006 Ecological collapse | Ecology | Economy, Defense | Constitutional ceilings, just transition, climate adaptation |
| RSK-007 Pandemic | Health | All | Standing preparedness, surge capacity, international coordination |
| RSK-008 Cyber attack | Technology | Infrastructure, Defense | Defense-in-depth, segmentation, mandatory standards, redundancy |
| RSK-010 AI misalignment | Technology | Governance, Defense | Risk-tiered regulation, audit, prohibition of autonomous lethal decisions |
| RSK-011 Foreign invasion | Defense | Economy, Ecology | Civil defense, alliances, resource sovereignty |
| RSK-014 Meaning crisis | Community | Health, Education | Community design, mental-health infrastructure, meaningful work, pluralism |
| RSK-024 Corporate concentration | Economy | Governance, Technology | Antitrust, interoperability, structural separation |
| RSK-030 Coup or self-coup | Governance | Defense, Justice | Civilian control, constitutional court, multi-body emergency declarations |
| RSK-034 Observability creep | Technology | Governance, Justice | Cryptographic separation, member observability of own data, periodic audit |

## Quantitative Constraints (illustrative)

These are framework-level targets. Specific numbers will be calibrated in simulation and pilots.

### TAR-Q1 Inequality

- Gini coefficient (post-tax-transfer): target below 0.30.
- Top-decile income share: target below 25%.
- Wealth concentration: declining trajectory, with structural limits on dynastic transmission.

### TAR-Q2 Ecology

- Carbon: net-zero by date set in ECN-B1; declining trajectory.
- Material footprint: trajectory toward sustainable per-capita levels.
- Biodiversity intactness: at or above 0.85 (or local equivalent).
- Water: withdrawals below sustainable yield in every watershed.

### TAR-Q3 Health

- Healthy life expectancy: monotonic improvement.
- Mental-health treatment access: within 30 days for non-urgent; same day for urgent.
- Loneliness rate: below specified threshold by age group.

### TAR-Q4 Governance and Rights

- Trust in institutions: monotonic improvement; reference levels above current OECD median.
- Procedural fairness perceptions: above baseline.
- Rights-violation rate: declining trajectory.

### TAR-Q5 Education

- Universal completion of upper secondary or equivalent.
- Adult-literacy and numeracy at OECD-leading levels.
- Inter-generational mobility above baseline.

### TAR-Q6 Resilience

- Reserve durations: per VAL-004 and ECN-IC2.
- Recovery times from defined shocks: targets per category.

## Open Issues

- Quantitative targets (TAR-Q) are illustrative; calibration depends on starting conditions of any specific polity adopting the framework.
- Inter-subsystem data minimization (TAR-DF) is bandwidth-constrained: too strict, and coordination fails; too loose, and surveillance creeps. Periodic review by GOV-B5.
- Multi-tier subsidiarity (TAR-P1) is intuitive but produces continuous coordination cost; the framework accepts this cost as the price of distributed authority.
- The architecture relies on adversarial review (TAR-P6) doing serious work; if that body atrophies, much of the design's protection weakens.
- The framework assumes substantial technical and administrative capacity in public sector; weak public-sector capacity is a transition risk addressed in ART-024.
- Behavioral targets (especially trust, loneliness) (TAR-Q3, TAR-Q4) depend on cultural conditions that institutions can influence but not fully determine.

## Cross-References

- All architecture modules ART-008 through ART-017.
- ART-019 (simulation blueprint) operationalizes this architecture for testing.
- ART-024 through ART-026 (implementation) translates this architecture into adoption paths.
- ART-031 (adversarial review) critiques this architecture systematically.
