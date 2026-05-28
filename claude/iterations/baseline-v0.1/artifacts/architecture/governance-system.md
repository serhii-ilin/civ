# Governance System

Artifact ID: ART-009
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: MOD-GOV
Depends on: ART-008

## Purpose

Specify the governance architecture: which bodies exist, what powers they hold, how members are selected, how power is constrained, how decisions are made, how disputes resolve, and how the system corrects itself. The design targets the values in `value-constitution.md` (ART-008) and is bound by the failure modes in `failure-mode-register.md` (ART-006).

The defining principle is *distributed authority with redundant checks*: no single body, person, or process can sustain a captured outcome against the others. Authority is multi-scale, multi-modal (elected, sorted, qualified, judicial), and time-rotated.

## Design Heuristics

From `behavioral-foundations.md` (ART-007) and `failure-mode-register.md` (ART-006):

- Distribute and rotate authority (lessons from BMK-001, BMK-003, BMK-004; RSK-001, RSK-002).
- Make procedural fairness enforcement-grade (B-002, CLM-090).
- Provide multi-modal participation (voting, deliberation, sortition) (CLM-018, CLM-102).
- Build standing feedback channels (RSK-003, RSK-019, RSK-043).
- Limit emergency powers explicitly (RSK-002, RSK-035, TZ-001).
- Couple competence with democratic legitimacy (TZ-005).
- Subsidiarity by default, universal rights as ceiling (TZ-006).

## Tier Structure (GOV-T)

The framework uses three primary tiers, each with subsidiary structures.

### GOV-T1 Local Cell

- Scale: roughly 5,000 to 50,000 members. Within Dunbar layering bounds (CLM-062, B-007) at upper end; small enough for direct participation at lower end.
- Bodies: Local Council (mixed elected and sorted); Local Manager (qualified executive); Local Ombuds; Local Conflict Forum.
- Powers: zoning, primary education delivery, local infrastructure, local commons management, conflict mediation, community-safety governance (not direct policing operations), local budget allocation within tier-2 envelope.

### GOV-T2 Regional Federation

- Scale: roughly 50,000 to 5 million members.
- Bodies: Regional Assembly (mixed); Regional Executive (qualified, multi-person); Regional Court; Regional Sortition Chamber; Regional Ombuds; Regional Audit Office.
- Powers: economic regulation within national framework, healthcare delivery, secondary education, regional infrastructure, regional ecological management, conflict resolution between local cells, regional emergency response.

### GOV-T3 National (and supra-national interfaces)

- Scale: tens of thousands to hundreds of millions.
- Bodies: detailed in Section "Bodies" below.
- Powers: defense, monetary policy, constitutional review, international relations, infrastructure of national scale, framework-wide standards.

### Subsidiarity Rule

Any power not explicitly enumerated to a higher tier is held by the lower tier. The constitution lists which powers are exclusively held at each tier; the rest are presumed local.

### Inter-tier Coordination

- Standing Federal Council: rotating representatives from regional assemblies meet quarterly to coordinate, propose framework-wide rules, and channel concerns upward.
- Conflict-of-tiers tribunal: cross-tier conflicts go to a mixed panel including national judicial and regional ombuds members.

## Bodies (GOV-B)

The following bodies exist at the national tier; analogous bodies exist at regional and (where applicable) local tiers.

### GOV-B1 Citizens' Assembly (sorted, deliberative)

- Composition: 400 members selected by stratified random sortition matching the demographic profile of the polity. Term: 18 months staggered so 1/3 rotate each 6 months.
- Powers: deliberate on contested policy questions; propose legislation; conduct mandatory review of policy areas on a rolling cycle; veto power on specified categories with supermajority (3/5).
- Procedures: structured deliberation with multi-perspective expert testimony; public transcripts and rationales; conflict-of-interest declarations.
- Capture defenses: random selection, short term, paid participation, expert pool with transparent selection, sortition body cannot succeed itself.

### GOV-B2 Representative Assembly (elected, multi-method)

- Composition: 500 members, elected via mixed-member proportional representation with district-level representation and party-list proportionality.
- Term: 4 years, staggered so 1/2 elected every 2 years.
- Powers: legislation; budget approval; executive oversight; declaration of emergencies (subject to GOV-B3, GOV-B5, GOV-B7 checks).
- Capture defenses: campaign-finance limits with public matching funds; rapid disclosure; per-member outside-income caps; recall by district referendum; revolving-door restrictions extending 4 years post-service.

### GOV-B3 Constitutional Court

- Composition: 11 justices selected via mixed nomination: 3 by the elected assembly (supermajority), 3 by the sortition assembly, 3 by the legal profession's independent body, 2 by the regional assemblies acting jointly.
- Term: single non-renewable 12-year term, staggered.
- Powers: judicial review of legislation against the constitution; review of emergency declarations; resolution of inter-body conflicts; rights enforcement.
- Capture defenses: mixed nomination, single non-renewable term, public reasoning requirement, ethics oversight by adversarial-review body.

### GOV-B4 Executive Council

- Composition: 7-member collective executive. Chair rotates annually. Members are selected for competence in distinct portfolios (security, economy, ecology, health, education, technology, social affairs).
- Selection: nominated by Representative Assembly, confirmed by Citizens' Assembly, ratified by Constitutional Court for competence and constitutional fitness.
- Term: 6 years, single renewable term, staggered so members rotate.
- Powers: executive administration; budget proposal; foreign policy execution; emergency response coordination subject to GOV-B2 and GOV-B3 review.
- Capture defenses: collective decision-making, rotation of chair, no single member can act unilaterally on framework-critical matters, every decision logged in publicly auditable register.

### GOV-B5 Adversarial Review Body

- Composition: 21 members; selected for adversarial-thinking capability and institutional independence (former judges, journalists, ombuds, civil society figures, academics). Mixed appointment by GOV-B1, GOV-B2, GOV-B3.
- Term: 8 years, single non-renewable.
- Powers: standing authority to investigate any institution, demand documents, publish findings, refer for prosecution, recommend removal of officials; access to classified materials with personal liability for misuse; binding authority on procedural compliance.
- Capture defenses: members nominated by multiple bodies; mandate to disagree with consensus; protected funding; cannot be dissolved without constitutional amendment.

### GOV-B6 Sortition Chamber

- Same as GOV-B1 but with specific powers in the constitutional architecture beyond deliberation: confirms executive appointments; conducts confirmatory referenda on contested legislation; participates in constitutional review.

### GOV-B7 Future Generations Advocate

- Composition: 7-member panel; appointed for staggered 10-year terms by mixed bodies; mandated to represent the interests of people 20+ years in the future.
- Powers: required to publish impact statements on long-horizon decisions; consultative role on infrastructure, ecological, and fiscal decisions; can refer to Constitutional Court for review of decisions with severe long-horizon impact.
- Capture defenses: long term, single non-renewable appointment, mandated criteria, public reasoning, independent secretariat.

### GOV-B8 Audit and Statistical Office

- Composition: career civil service led by an Auditor General with single 10-year term.
- Powers: audit all public bodies and major private bodies receiving public funds; produce national statistics; publish institutional dashboards; provide framework-wide data infrastructure.
- Capture defenses: career civil-service protection for staff, independent funding, mandatory public reporting, criminal liability for falsification.

### GOV-B9 Ombuds Network

- Composition: ombuds at each tier; coordinating Ombuds General at national level; specialized ombuds for children, elders, disabled members, prisoners, asylum seekers, military personnel.
- Powers: receive complaints; investigate; mediate; refer to courts or adversarial-review body; publish patterns.
- Capture defenses: independent funding; reporting line to legislature, not executive; whistleblower protection extended to staff.

### GOV-B10 Independent Regulators

- Independent commissions for: central bank, electoral commission, anti-corruption commission, data-protection authority, public-service broadcaster, antitrust authority, environmental regulator, electoral commission, AI safety regulator.
- All have: mixed-body appointments, fixed terms, public reasoning, mandatory reporting, audit by GOV-B8.

### GOV-B11 Federal Council of Regions

- Composition: rotating representatives from regional assemblies (GOV-T2 bodies); rotated annually; 2 members per region.
- Powers: review national legislation for regional impact; veto in specific cases (constitutionally enumerated); coordinate inter-regional matters.
- Capture defenses: short tenure, mandate from regional assemblies, sunset on its own rules.

## Selection Methods (GOV-S)

The framework uses four selection methods. Each role uses one or a mix.

### GOV-S1 Stratified Sortition

- Random selection from member rolls, stratified by demographic dimensions specified by constitution (age, gender, region; not by political affiliation).
- Service is compensated and protected; opting out requires hardship attestation.
- Used in: GOV-B1, GOV-B6, citizen juries, participatory budgeting panels.
- Caveat (CLM-018): durability at large scale untested; framework hedges with non-sortition bodies in parallel.

### GOV-S2 Mixed-Member Proportional Election

- District-level representatives plus party-list proportional members.
- Public campaign finance with limits and rapid disclosure.
- Used in: GOV-B2, regional assemblies.

### GOV-S3 Qualified Appointment

- Nomination by one body, confirmation by another, ratification or veto by a third where applicable.
- Qualifications: transparent criteria, written exams or portfolio assessments where applicable, peer evaluation.
- Used in: GOV-B3, GOV-B4, GOV-B10, judges, regulators, executive department heads.
- Caveat (VAL-006): qualification systems can themselves be captured (credentialism); design must use multi-method assessment, transparent rubrics, and bias audits.

### GOV-S4 Career Civil Service

- Open competitive hiring; merit-based promotion; tenure protection; non-political ethos.
- Used in: GOV-B8 staff, GOV-B9 staff, line ministries, regulators.

## Decision Rules (GOV-D)

### GOV-D1 Ordinary Legislation

- Originated in GOV-B2 or proposed by GOV-B1.
- Passed by majority of GOV-B2.
- Subject to GOV-B6 confirmatory referendum if requested by 5% of citizens or by 1/3 of GOV-B2 minority.
- Subject to GOV-B3 review for constitutional compliance.

### GOV-D2 Constitutional Amendment

- Originated by GOV-B2 or GOV-B6.
- Requires 2/3 of GOV-B2, 2/3 of GOV-B6, 3/4 of regional assemblies (a majority in each), and ratification by citizen referendum or sortition assembly.
- 90-day public deliberation period.
- Adversarial review by GOV-B5 before final vote.

### GOV-D3 Budget

- Drafted by GOV-B4; reviewed by GOV-B2; approved by GOV-B2 majority.
- Multi-year framework with annual operating; ecological-impact statement and long-horizon-impact statement (GOV-B7) required.
- Audited by GOV-B8.

### GOV-D4 Treaty and War Powers

- Treaties negotiated by GOV-B4, ratified by 3/5 of GOV-B2.
- Declarations of war require 2/3 of GOV-B2 plus 3/5 of GOV-B6.
- Use of force without prior declaration (in cases of imminent threat) requires reporting to GOV-B2 within 48 hours and ratification within 14 days.

### GOV-D5 Emergency Powers

- Declared by GOV-B4; ratified within 14 days by 3/5 of GOV-B2 (or expires).
- Default expiry: 30 days. Maximum renewal: cumulative 180 days without 2/3 reauthorization.
- Each renewal requires public report on necessity and proportionality.
- GOV-B5 has continuing oversight; GOV-B3 has continuing judicial review.
- Non-derogable rights (VAL-001) hold throughout. (Bound by TZ-001.)

## Member Observability (GOV-O)

In line with VAL-019, members of the polity must be able to see what their institutions are doing without being surveilled in return. Specifications below are binding on every governance body.

### GOV-O1 Public Decision Logs

- Every decision of GOV-B2, GOV-B3, GOV-B4, and GOV-B10 is logged in machine- and human-readable form within 30 days. Includes: deciding body, decision, alternatives considered, evidence cited, dissenting opinions, expected impact.
- Closed sessions are permitted only for narrow defined reasons (personnel; security; ongoing litigation); the existence of the closure and its category are public; the decision itself is published when the reason expires.

### GOV-O2 Institutional Dashboards

- Each body publishes a real-time dashboard: budget execution, staffing, decision throughput, decision latency, error rate, complaint volume, complaint resolution time, audit findings, key program metrics.
- Dashboards are accessible without login, in plain language and machine-readable form.

### GOV-O3 Auditable Algorithms

- Any algorithmic system used by a public body that affects rights or material outcomes must be documented, audited, and inspectable per `technology-and-ai-governance.md` (ART-016).

### GOV-O4 Personal Data Protection

- Member observability covers institutions, not individuals. Personal data is aggregated for institutional accountability; raw personal data is never published. (Bound by TZ-004 and VAL-015.)

### GOV-O5 Transparency Limits

- Information categorized as classified (security, witness protection, ongoing investigations, deliberative pre-decisional) is limited; access is granted to GOV-B5 (adversarial review) and GOV-B8 (audit) with personal liability for misuse.
- Classification categories are limited by statute; over-classification is itself a violation reportable to GOV-B5.

## Anti-Capture Provisions (GOV-A)

### GOV-A1 Financial Disclosures

- All elected officials, appointed officials, regulators, judges, and senior civil servants publish complete financial holdings, sources of income, and major gifts annually. Family members in the same household covered.
- Conflict-of-interest assessment is automatic; recusal triggers documented.

### GOV-A2 Revolving-Door Restrictions

- Officials with regulatory power may not work for or consult to regulated industries for 4 years after leaving office.
- Officials with procurement authority subject to comparable restrictions.

### GOV-A3 Lobbying Transparency

- Any meeting with elected or appointed officials by lobbyists or interest representatives is logged: who, when, on whose behalf, on what topic. Logged within 7 days.
- "Lobbyist" is broadly defined to include corporate, civil-society, and foreign actors.

### GOV-A4 Campaign Finance

- Public matching funds available for qualifying candidates; private contributions capped per donor per cycle; foreign and corporate political donations prohibited.
- Real-time disclosure of donations above a threshold.

### GOV-A5 Audit Independence

- GOV-B8 funding is constitutionally protected at a percentage of national budget; cannot be reduced without supermajority of GOV-B2 and GOV-B6.

### GOV-A6 Whistleblower Protections

- Strong legal protections; protected reporting channels to GOV-B5 and GOV-B9; criminal penalties for retaliation; financial support for whistleblowers facing economic consequences.

### GOV-A7 Anti-Hereditary Provisions

- No transmission of political office by family relationship is allowed; constitutionally prohibited.
- Immediate-family conflicts of interest disclosed and recused.

### GOV-A8 Capture-Resistance Audit

- GOV-B5 publishes an annual capture-resistance audit assessing concentration of power, regulator-industry relationships, judicial independence, and information environment.

## Accountability and Removal (GOV-R)

- Recall: district-elected GOV-B2 members are subject to recall by district petition (15% of district) and confirmatory vote.
- Impeachment: GOV-B4 members impeachable by GOV-B2 (majority) plus GOV-B6 (majority); removal requires GOV-B3 finding of constitutional violation, criminal conduct, or gross incompetence.
- Judicial removal: GOV-B3 justices removable by GOV-B2 (2/3) plus GOV-B6 (2/3) on impeachment articles drafted by GOV-B5.
- Regulator removal: limited grounds (specific cause), high threshold, public reasoning.
- Election fraud: criminal offense; ineligibility to hold office; possible dissolution of party.

## Crisis and Continuity (GOV-C)

### GOV-C1 Order of Succession

- Continuity-of-government plans are constitutionally specified; rehearsed annually.
- No single-point-of-failure in leadership.

### GOV-C2 Decision-Making Under Disruption

- Pre-authorized emergency-decision frameworks specify who decides what under which disruption profile.
- Authority reverts to normal channels at the earliest opportunity; revert is automatic, not at the discretion of crisis authority.

### GOV-C3 Loss of Quorum

- If GOV-B2 cannot meet, GOV-B6 takes interim deliberative role; GOV-B3 retains review authority; emergency authority constrained.

## Inter-Body Conflicts (GOV-I)

- Conflicts between GOV-B2 and GOV-B4 are mediated by GOV-B3.
- Conflicts between GOV-B1/B6 and GOV-B2 are mediated by GOV-B3; sortition rulings on constitutional questions of legitimacy have heightened weight.
- Conflicts between national and regional tiers resolved by GOV-B3 with GOV-B11 input.
- Conflicts among regulators (GOV-B10) coordinated by GOV-B4 with appeal to GOV-B3.

## Performance Metrics (GOV-M)

Dashboards (GOV-O2) include at minimum:

- Decision latency by issue category.
- Public participation in deliberative processes.
- Trust in institutions (multiple measures).
- Perceived procedural fairness (sampled).
- Appeals success rate.
- Audit findings response time.
- Whistleblower retaliation incidents.
- Lobbyist meeting density per official.
- Implementation gap between law and observed compliance.
- Long-horizon impact statement coverage.

Indicators are designed with Goodhart-Campbell caution (CLM-189): no single indicator drives a budgetary or staffing decision; indicators are audited for distortion regularly.

## Open Issues

- Specific sortition durability at national scale (CLM-018) is empirically thin; the design hedges with mixed bodies. A future iteration should pilot at regional scale before scaling.
- Boundary between competence-gated and democratic roles (TZ-005) is operationalized here per role; future review should test whether the cut points produce capture or function failure.
- Emergency-power thresholds (GOV-D5) are conservative; regional contexts with frequent natural disasters may need calibrated variants.
- Member observability infrastructure (GOV-O) is technically specified in ART-016; the present artifact is normatively binding but operationally dependent on that infrastructure.
- The framework's stance on parties (de facto allowed via GOV-S2) and party regulation (de facto by GOV-A4) is minimal; future iterations may add stronger party-law specifications.

## Cross-References

- Bound by: VAL-001, VAL-005, VAL-006, VAL-007, VAL-008, VAL-015, VAL-018, VAL-019.
- Coordinates with: ART-011 (law), ART-016 (tech), ART-017 (defense), ART-019 (simulation), ART-024 (implementation), ART-026 (migration).
- Tested in: simulation scenarios for elite capture, demagogue ascent, judicial pressure, emergency-power ratchet, sortition durability.
