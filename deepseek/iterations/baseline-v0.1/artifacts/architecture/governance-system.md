# ART-009: Governance System Architecture

Iteration: `baseline-v0.1`
Status: draft

## Purpose

Design a capture-resistant, legitimate, competence-aware, self-correcting governance system organized as a federated multi-tier architecture with hybrid representation (electoral, sortition-based, and expertise-advisory).

## System Overview

The governance system is organized in three principal tiers:

1. **Community Cell** (100-300 residents): Face-to-face deliberative governance
2. **Regional Federation** (50-200 community cells): Coordination of regional services, infrastructure, and cross-community disputes
3. **National/Central Governance**: Constitutional enforcement, defense, currency, external relations, and inter-regional equity

Each tier has a defined scope of authority. Powers not explicitly delegated upward remain at the lowest tier (subsidiarity). The architecture is explicitly federal, with dual legitimacy from (a) individual citizens and (b) community/regional bodies.

## Tier 1: Community Cell Governance

### Scope
- Local public space, community-scale infrastructure
- Community dispute resolution (pre-formal justice)
- Mutual aid and community care coordination
- Local land-use decisions within regional framework
- School governance (within national education standards)
- Local cultural and civic events
- Community-level observability reporting (wellbeing metrics, conflict outcomes, resource flows)

### Structure
- **Community Assembly**: All adult residents, meeting monthly. Decisions by deliberative consensus where possible, supermajority vote (60%) where consensus fails. Quorum: 25% of eligible residents.
- **Community Council**: 5-9 members selected by stratified random sortition (demographically representative sample). 2-year terms, staggered. Council manages assembly agenda, executes assembly decisions, and coordinates with regional bodies. No consecutive terms.
- **Community Auditor**: Independent role, externally appointed, reporting to regional accountability body. Audits community finances, decisions, and compliance with constitutional values.
- **Community Health Advocate**: Appointed by assembly, reports on community wellbeing metrics, isolation, care gaps, and trauma exposure.

### Competence Mechanisms
- Assembly members receive deliberation training (half-day) and issue briefs before substantive meetings.
- Council members receive governance training (2-week program) before taking office.
- Facilitated deliberation by trained neutral facilitators (rotating, not community members).
- Expert advisors available on request from regional knowledge pool.

### Observability
- All assembly and council minutes published within 48 hours.
- Community budget and expenditure publicly visible in real time.
- Wellbeing dashboard: community-level aggregated metrics (loneliness, care burden, conflict incidents, resource flows, institutional response times).
- Personal data never exposed: all metrics are aggregated and anonymized.

### Anti-Capture Mechanisms
- Sortition prevents wealthy/influential individuals from monopolizing community council.
- Compulsory attendance allowance (standard hourly rate) removes economic barrier to participation.
- Assembly decisions can be challenged by any 10 residents and reviewed by regional governance ombuds.
- Community auditor independence enforced by external appointment.

**Decision**: DEC-GOV-001 (community scale set at 100-300 based on Dunbar-scale research and deliberative-democracy evidence). Rationale: face-to-face deliberation quality degrades above ~300; below ~100, diversity and capability insufficient for resilience functions.

---

## Tier 2: Regional Federation

### Scope
- Regional infrastructure (transport, energy distribution, water management, waste)
- Police oversight and public-safety coordination
- Regional healthcare network coordination
- Cross-community dispute resolution
- Regional economic coordination and labor-market policy
- Ecological monitoring and land-use framework
- Regional education coordination (standards implementation)
- Regional disaster response and civil defense

### Structure
- **Regional Assembly**: Hybrid body of 100-200 members:
  - 50%: Community delegates (elected by community assemblies, proportional representation)
  - 30%: Stratified random sortition from regional citizenry
  - 20%: Competence-gated appointments (subject-matter experts selected through transparent competency assessment)
- **Regional Executive Council**: 7-13 members elected by regional assembly from its ranks, with constraints:
  - No single party/coalition may hold >60% of seats
  - Professional qualification requirements for relevant portfolios (infrastructure, health, public safety, finance)
  - 4-year terms, maximum 2 terms
- **Regional Constitutional Court**: 5-7 judges with 12-year non-renewable terms. Appointed by 2/3 regional assembly vote from a shortlist prepared by an independent judicial-nominations commission.
- **Regional Audit and Anti-Corruption Office**: Independent body with prosecutorial referral power. Director appointed by 2/3 vote for single 10-year non-renewable term.
- **Regional Citizen Oversight Panel**: 15-25 randomly selected citizens serving 1-year terms, with access to all regional government records, authority to commission investigations, and obligation to publish quarterly public reports.

### Competence Mechanisms
- Executive Council candidates for technical portfolios must pass competency assessment administered by independent professional body.
- All candidates for any office must complete public ethics and governance training.
- Performance audits conducted annually by Regional Audit Office; results published.
- Citizen Oversight Panel provides continuous public scrutiny.

### Observability
- All regional assembly votes recorded and published.
- Regional budget: real-time expenditure tracking, open procurement portal.
- Enforcement dashboard: policing actions, complaint outcomes, use-of-force incidents (anonymized to protect victims and officers, but aggregated and searchable).
- Institutional-performance dashboard: service-delivery metrics, response times, citizen-satisfaction scores, complaint-resolution rates.
- Regional-risk dashboard: ecological indicators, fiscal health, social-cohesion metrics, external-boundary integrity.

### Anti-Capture Mechanisms
- Mixed representation (sortition, electoral, expert) prevents any single group from dominating.
- Compulsory disclosure of all meetings between elected officials and non-governmental entities.
- Post-employment cooling-off: 2-year minimum before former officials can work in industries they regulated.
- Public financing of electoral campaigns (no private donations).
- Regional anti-corruption office with guaranteed budget indexed to inflation and population (insulated from political budget cycles).

**Decision**: DEC-GOV-002 (mixed-representation model). Rationale: pure sortition lacks accountability mechanisms; pure electoral reproduces elite overrepresentation (CLM-040). Hybrid model balances legitimacy (electoral mandate), diversity (sortition), and competence (expert appointments).

---

## Tier 3: National/Central Governance

### Scope
- Constitutional interpretation and enforcement
- Defense and external security
- Monetary policy and currency
- External relations, treaties, and trade policy
- Inter-regional equity and redistribution
- National infrastructure coordination (grid interconnection, major transport)
- Immigration, asylum, and border governance
- Biosecurity and pandemic response
- Technology and AI governance standards
- National data-rights framework
- Emergency powers (declaration, management, and termination)

### Structure
- **National Assembly**: 200-400 members:
  - 40%: Electoral representatives from regions (proportional representation, open-list)
  - 40%: Stratified random sortition from national citizenry
  - 20%: Competence-gated appointments (domain experts selected through transparent assessment)
  - All serve 3-year terms with 2-term limit
- **National Executive**: 5-9 members elected by National Assembly, serving as collective head of government.
  - Portfolio-specific competency requirements
  - No single party/coalition may hold >60% of executive seats
  - 4-year terms, maximum 2 terms
- **Constitutional Court**: 9 judges, 15-year non-renewable terms. Appointment by 2/3 National Assembly vote from independent nominating commission shortlist. Jurisdiction: constitutional review, fundamental-rights protection, inter-tier disputes.
- **National Audit and Anti-Corruption Authority (NACA)**: Highest anti-corruption body. Director appointed by 3/4 Constitutional Court vote for single 12-year non-renewable term. Own budget indexed to GDP. Prosecutorial independence.
- **Observatory of Institutional Health (OIH)**: Independent agency monitoring all governance tiers for capture risk, corruption, competence decline, and democratic backsliding. Publishes annual Institutional Health Report. Director appointed by 2/3 National Assembly from shortlist prepared by independent academic panel.
- **National Civil Defense Council**: Coordinates defense, disaster response, and resilience across regions. Civilian-controlled with military reporting to civilian leadership.

### Competence Mechanisms
- National Assembly expert-appointee seats require demonstrated domain expertise (publications, professional credentials, peer review) assessed by independent academic/professional body.
- Executive portfolio-holders must pass competency examination administered by independent professional association.
- All authority-bearing positions subject to annual fitness review (physical, cognitive, ethical) by independent medical/psychological board.
- Competency standards publicly available; assessment results appealable.

### Anti-Capture Mechanisms
- Multiple representation channels prevent single capture vector.
- NACA with guaranteed budget and prosecutorial independence.
- OIH acts as early-warning system for institutional degradation.
- Public financing for all electoral campaigns; strict limits on all other political spending.
- Mandatory asset declarations updated annually, publicly accessible, with criminal penalties for false declaration.
- Parliamentary ethics committee with opposition majority (committee chair from largest non-government party).
- Compulsory public logging of all meetings between officials and external parties.
- Strict revolving-door enforcement: 3-year cooling-off for ministers, 2-year for senior officials.
- Unexplained-wealth orders: officials whose assets cannot be explained by declared income face confiscation.

**Decision**: DEC-GOV-003 (NACA independence model). Rationale: CLM-043 shows structural independence (prosecutorial autonomy, guaranteed budget, competitive selection) is the most effective anti-corruption mechanism. Political budget control is the most common capture vector.

---

## Core Institutional Mechanisms

### Sortition System
- **Pool**: All adult citizens, with opt-out for conscientious objection (requires alternative civic service).
- **Stratification**: Random samples stratified by region, age cohort, gender, and socioeconomic indicators to ensure demographic representativeness.
- **Compensation**: Full wage replacement (up to cap) for service period.
- **Training**: Intensive 2-week governance and deliberation training before service.
- **Expert access**: Unrestricted access to expert advisors, evidence briefs, and adversarial analysis.
- **Rotation**: Terms are non-renewable within 6 years.

### Competence-Gating System
- **What it gates**: Technical portfolio-holder positions in executive; expert-appointee seats in assemblies; judges; auditors; senior regulators.
- **What it does NOT gate**: Electoral representatives; sortition representatives; citizens' assembly membership; voting rights; civic participation.
- **Assessment method**: Independent professional bodies develop and administer assessments. Assessments test demonstrated knowledge and skill, not credentials. Portfolios available for public scrutiny.
- **Anti-capture**: The assessment body is itself subject to NACA audit and OIH review. Assessment standards are publicly available and legally challengeable.

### Adversarial Review Body
- **Permanent Constitutional Review Commission**: 11 members serving 8-year terms. Half appointed by Constitutional Court, half by National Assembly (2/3 vote). Permanent adversarial review body with authority to:
  - Inspect any governance decision for constitutional compliance
  - Commission investigations
  - Publish findings (cannot be suppressed)
  - Refer violations to Constitutional Court or NACA
  - Propose constitutional amendments
  - Review emergency powers every 30 days during declared emergencies

### Emergency Powers Architecture
- **Declaration**: National Executive may declare emergency for 30 days with 3/4 National Assembly approval. Renewal requires 3/4 each 30 days.
- **Concurrent review**: Constitutional Review Commission reviews every 2 weeks.
- **Non-derogable rights**: Freedom from torture, extrajudicial killing, slavery, forced disappearance (VAL-001 non-derogable elements). Habeas corpus may be suspended only for 7 days at a time with judicial reauthorization.
- **Expiration**: Emergency powers expire after 180 days unless renewed by 3/4 National Assembly AND national referendum.
- **Post-emergency**: Mandatory 60-day review by Constitutional Review Commission with public report. All emergency actions reviewed for proportionality; violations prosecuted.

### Budget Architecture
- **Participatory budgeting**: Regional and community tiers allocate 15-30% of discretionary budget through participatory processes.
- **Multi-year budgeting**: National budget operates on 3-year cycles with annual adjustments, reducing short-term political manipulation.
- **Automatic stabilizers**: Certain expenditures (health, education, anti-corruption, observability infrastructure) are indexed to population, inflation, and need indicators, removing them from annual political negotiation.
- **Transparency**: All budgets, expenditures, procurement contracts, and grant recipients publicly searchable in real time.

---

## Decision Log: Governance

| Decision ID | Scope | Decision | Alternatives | Rationale | Evidence | Revisit Trigger |
| --- | --- | --- | --- | --- | --- | --- |
| DEC-GOV-001 | Community scale | 100-300 persons | 30-100 (more intimate), 500-5000 (more efficient service delivery) | Face-to-face deliberation quality (CLM-011); Dunbar-scale limits (BF-004); community-cohesion evidence (CLM-030) | SRC-014, SRC-090, SRC-095 | Simulation results showing significant performance difference at alternative scales |
| DEC-GOV-002 | Representation model | Hybrid: electoral (40%) + sortition (40%) + expert (20%) | Pure electoral, pure sortition, different ratios | Electoral alone reproduces elite bias (CLM-040); sortition lacks accountability; expert alone creates technocracy. Hybrid balances legitimacy, representativeness, and competence. | SRC-090, SRC-010, CLM-040 | Evidence of systematic failure in any single channel |
| DEC-GOV-003 | Anti-corruption authority | Independent body with prosecutorial power, guaranteed budget, 12-year director term | Parliamentary committee, independent-auditor-only, judiciary-embedded | CLM-043: structural independence + prosecutorial power most effective. Political budget control is capture vector. | SRC-034, SRC-011 | Capture of NACA itself (detected by OIH) |
| DEC-GOV-004 | Emergency-powers architecture | 30-day renewable with concurrent independent review; non-derogable core rights; automatic expiration | Permanent emergency provisions, stricter limits, more flexible powers | Balance between crisis-response capability and rights protection (RSK-014). Multiple independent review layers prevent normalization. | SRC-086, RSK-014 | Historical precedent showing 30-day window too short for declared emergency types |
| DEC-GOV-005 | Competence-gating scope | Technical executive portfolios + expert assembly seats; does NOT include voting, candidacy, or citizen-assembly participation | No competence-gating, broader gating | VAL-007 requires competence with accountability. Narrow gating prevents credential cartels while ensuring technical competence where it affects public safety and institutional function. | SRC-090, CLM-040 | Credential-cartel formation detected by OIH |

---

## Cross-Module Interfaces

| Interface | Partner Module | Coordination Requirement |
| --- | --- | --- |
| Law and justice | MOD-LAW | Constitutional Court jurisdiction, legal-system independence, rights enforcement, observability legal framework |
| Economy | MOD-ECO | Tax authority, fiscal policy, commons management, economic governance, beyond-GDP metrics |
| Technology | MOD-TAI | AI governance limits, digital infrastructure, observability technology, cybersecurity |
| Defense | MOD-DEF | Civilian-military relations, emergency powers scope, defense oversight, external boundary governance |
| Community | MOD-CUL | Community-cell governance alignment, civic identity, cultural autonomy bounds |
| Ecology | MOD-ECOINF | Ecological governance integration, land-use jurisdiction, resilience standards |
| Health | MOD-HMH | Health-governance interface, public-health emergency powers, healthcare governance |
| Education | MOD-EDU | Education governance, curriculum standards, teacher certification |

## Unresolved Questions

- RQ-GOV-001 (from module): Which powers must be local, regional, or central? (Architectural answer provided here but requires simulation validation.)
- RQ-GOV-002: Competence assessment methodology requires further specification to prevent credential capture.
- RQ-GOV-005: Minority-rights protection during crisis needs stress-testing through simulation (MOD-SIM).
- RQ-GOV-006: Observable vs. private data classification needs detailed legal specification (MOD-LAW coordination).