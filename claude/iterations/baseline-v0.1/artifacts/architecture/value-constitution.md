# Value Constitution

Artifact ID: ART-008
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: all
Depends on: canon/values.md

## Status of This Document

This is a formal, operational expansion of the value constitution in `canon/values.md`. Where this artifact and the canon document differ, the canon is authoritative. This artifact adds: precise definitions, indicators with measurement notes, conflict-resolution procedures, amendment procedures, value-tradeoff zones, and a binding interpretation table that downstream architecture modules must respect.

All architecture, simulation, and implementation artifacts in this iteration are bound by this constitution. Any proposed design choice that would violate a value here must be flagged as a contradiction (see ART-029) and either revised or proposed as a constitutional amendment.

## Article I: Preamble

This framework exists to serve the dignity, capability, health, freedom, and durable wellbeing of its members, and to do so within ecological limits, across generations, and through institutions that are observable, contestable, and capable of self-correction.

The framework rejects:

- Any design that requires permanent good will of leaders to function.
- Any design that requires permanent absence of bad actors to function.
- Any design that traps people in institutions they cannot leave or reform.
- Any design that exports its costs onto future generations, marginalized groups, or non-human nature.
- Any design that becomes legible only to experts and opaque to members.

## Article II: Core Values

The values from `canon/values.md` (VAL-001 through VAL-019) are adopted in full. This article restates them with operational expansion. The canonical IDs remain stable.

### VAL-001 Human Dignity and Rights

- Operational definition: every member possesses inherent worth, bodily autonomy, freedom of conscience, due process, and protection from arbitrary coercion.
- Non-derogable elements: protection from torture, slavery, arbitrary detention, summary execution; freedom of conscience; due process; ability to seek legal review.
- Bound by: VAL-008 (legal protection); VAL-010 (pluralism); VAL-015 (privacy).
- Primary indicators: rights-violation rate (per 100,000 members, by type); access to legal representation; due-process completion rate; minority-rights audit results.
- Measurement caveat: under-reporting is universal; multiple data sources required.

### VAL-002 Health by Design

- Operational definition: physical, mental, relational, and societal health are designed-in structural goals, not downstream consequences.
- Includes: built environment, food and water systems, work conditions, community infrastructure, healthcare access, mental health provision.
- Bound by: VAL-012 (mental health); VAL-015 (privacy in health data); VAL-017 (care infrastructure).
- Primary indicators: life expectancy at birth and at 65; healthy life expectancy; preventable disease burden; mental-health service access; loneliness rate; child wellbeing index; maternal mortality.
- Measurement caveat: distributional metrics required — averages can conceal severe inequality.

### VAL-003 Ecological Boundaries

- Operational definition: economic, industrial, and social systems must operate within planetary and local ecological limits.
- Binding constraints: greenhouse gas budget; biodiversity baseline; water budget by watershed; soil-quality maintenance; biogeochemical-flow limits.
- Bound by: VAL-014 (sustainable progress); VAL-016 (intergenerational stewardship).
- Primary indicators: material footprint per capita; carbon budget compliance; biodiversity intactness; water-stress index; land-use intensity; pollution loadings.
- Measurement caveat: planetary boundary methodology evolves; the framework binds to *direction* and to local ecological measurements with high confidence.

### VAL-004 Resilience as Architecture

- Operational definition: the society must survive, adapt, and recover from ecological, economic, military, technological, institutional, and cultural shocks.
- Specific requirements: redundant supply for water, food, energy, medical materials, communications; institutional continuity protocols; community-level reserve capacity.
- Bound by: VAL-013 (self-sufficiency); VAL-018 (self-correction); VAL-019 (boundary integrity).
- Primary indicators: recovery time from defined shocks; reserve duration for essentials; supply-chain concentration index; institutional-continuity drill outcomes.
- Measurement caveat: tested by exercise, not only by indicator; periodic stress tests required.

### VAL-005 Legitimate and Consent-Based Governance

- Operational definition: governance is competent, fair in procedure, contestable, and consent-based by the governed; not merely majoritarian.
- Includes: voting, deliberation, sortition, courts of appeal, recall, secession or exit pathways for substantial groups under defined conditions.
- Bound by: VAL-006 (capture resistance); VAL-008 (rule of law); VAL-010 (pluralism); VAL-018 (self-correction).
- Primary indicators: trust in institutions; turnout and participation; perceived procedural fairness; appeals-success rate; rights-removal rate.
- Measurement caveat: trust can be manufactured by suppression — pair trust metrics with rights metrics.

### VAL-006 Capture-Resistant Governance

- Operational definition: power concentration, nepotism, corruption, regulatory capture, and institutional capture are structurally constrained.
- Mechanisms: term and tenure limits; rotation; multi-body appointments; asset and meeting disclosure; revolving-door restrictions; independent enforcement.
- Bound by: VAL-007 (competence + accountability); VAL-019 (observability).
- Primary indicators: power-concentration indices; conflict-of-interest findings; lobbying transparency; enforcement independence audit; persistent-elite indicators across cohorts.
- Measurement caveat: capture is usually invisible to surface metrics; adversarial audit required.

### VAL-007 Competence with Accountability

- Operational definition: roles with public authority require verified competence, ethical fitness, transparent review, and removal mechanisms.
- Mechanisms: independent qualification verification; performance audit; recall and removal procedures; mandatory error reporting; protected whistleblowers.
- Bound by: VAL-005 (legitimacy); VAL-006 (capture resistance).
- Primary indicators: qualification-validity rate; performance-audit outcomes; recall and removal rates; error-correction time; whistleblower retaliation rate.
- Measurement caveat: competence assessment is a known capture vector (credentialism); design must avoid this.

### VAL-008 Justice and Rule of Law

- Operational definition: law is public, consistent, rights-protecting, proportionate, reviewable, and accessible to all.
- Mechanisms: clear and accessible statutes; independent judiciary; legal aid; restorative and rehabilitative options; appeals; time-limited emergency rules with review.
- Bound by: VAL-001 (rights); VAL-005 (legitimacy); VAL-010 (pluralism).
- Primary indicators: legal-access index; case duration; wrongful conviction rate; police-violence rate; restorative-resolution rate; equal-treatment audits.
- Measurement caveat: most jurisdictions under-report rights violations and over-report procedural completeness.

### VAL-009 Science-Guided Policy

- Operational definition: empirical questions are answered through evidence, with explicit uncertainty; moral tradeoffs remain democratic and constitutional.
- Mechanisms: evidence-grading discipline; replication requirement for high-stakes claims; public uncertainty disclosure; protected independent science institutions; explicit separation between empirical and normative claims in policy.
- Bound by: VAL-001 (rights as constraints on empirical claims); VAL-018 (self-correction).
- Primary indicators: evidence-classification compliance; uncertainty-disclosure rate; replication completion; conflict-of-interest disclosure.
- Measurement caveat: science institutions can themselves be captured; protections required.

### VAL-010 Pluralism and Freedom of Conscience

- Operational definition: religious, spiritual, philosophical, cultural, and lifestyle diversity is protected; no group has institutional supremacy.
- Mechanisms: separation of belief and state; equal access to public services and offices; protection from religious or ideological coercion; freedom to enter and exit groups; non-discrimination law.
- Bound by: VAL-001 (rights); VAL-008 (equal protection).
- Primary indicators: viewpoint-diversity audits; discrimination rates by group; exit-rate by community; cultural-participation indices.
- Measurement caveat: pluralism conflicts with anti-pluralist movements; constitutional response is rule-of-law enforcement, not group suppression.

### VAL-011 Education as Foundation

- Operational definition: education develops cognitive resilience, emotional intelligence, practical skill, civic literacy, and lifelong learning capacity.
- Mechanisms: early childhood services; equitably resourced public education; teacher quality; civic and statistical literacy; reskilling for adult workers; multilingual support.
- Bound by: VAL-013 (self-sufficiency); VAL-017 (care); VAL-018 (self-correction).
- Primary indicators: literacy, numeracy, critical thinking; civic-knowledge assessment; adult-learning access; teacher-retention; equity-gap closure.
- Measurement caveat: standardized assessment is one input only; pair with practical capability assessment.

### VAL-012 Mental Health as Civic Infrastructure

- Operational definition: psychological wellbeing is a public-infrastructure concern, not only an individual healthcare responsibility.
- Mechanisms: universal access to mental healthcare; community-level support; trauma-informed institutions; reduction of structural stressors; destigmatization in education and culture.
- Bound by: VAL-002 (health); VAL-015 (privacy); VAL-017 (care).
- Primary indicators: access to professional care; suicide and self-harm rates; trauma-exposure rates; treatment retention; community-support density.
- Measurement caveat: stigma suppresses reporting; multiple measurement modalities required.

### VAL-013 Self-Sufficiency and Chosen Interdependence

- Operational definition: members, families, communities, and larger systems are capable of basic independent function while choosing interdependence.
- Mechanisms: practical skill education; local production floors; community reserves; ability to operate during disruption.
- Bound by: VAL-004 (resilience); VAL-014 (sustainable progress).
- Primary indicators: local production capacity; household preparedness; community reserve duration; concentration of upstream dependencies.
- Measurement caveat: "self-sufficiency" is a directional concept here, not autarky; the framework is internationalist within boundary protections (VAL-019).

### VAL-014 Sustainable Progress Beyond GDP

- Operational definition: progress is measurable improvement in wellbeing, capability, resilience, justice, and ecological balance.
- Mechanisms: composite progress index, capability indicators, sustainable-development indicators alongside (not replacing) economic indicators; budget-impact statements against these metrics.
- Bound by: VAL-003 (ecological boundaries); VAL-016 (intergenerational).
- Primary indicators: wellbeing index; capability indices; HDI-like composites; genuine progress indicator; ecological balance.
- Measurement caveat: composite indicators distort; primary indicators must be inspectable too.

### VAL-015 Privacy and Data Rights

- Operational definition: transparency for institutions must not become surveillance of people; data collection is purpose-limited, consented, minimized, auditable.
- Mechanisms: constitutional data rights; purpose limitation; retention limits; mandatory algorithmic-impact assessment for high-stakes systems; member access to own data; warrant requirements for state access to personal data.
- Bound by: VAL-001 (rights); VAL-018 (self-correction); VAL-019 (observability for institutions, not people).
- Primary indicators: data-breach rate; surveillance-warrant rate and outcomes; consent-compliance audit; algorithmic-impact-assessment coverage; subject-access-request fulfillment.
- Measurement caveat: enforcement is the binding constraint, not legal text.

### VAL-016 Intergenerational Stewardship

- Operational definition: decisions protect rights, resources, institutions, and ecological base of future generations.
- Mechanisms: future-generations advocate institution; long-horizon impact statements; sovereign-wealth and pension-fund protection; infrastructure-maintenance budget protection; constitutional protection of ecological base.
- Bound by: VAL-003 (ecological); VAL-018 (self-correction).
- Primary indicators: long-term debt to GDP; ecological-debt accounting; infrastructure-maintenance backlog; youth-wellbeing metrics.
- Measurement caveat: future generations cannot vote; institutional advocacy required.

### VAL-017 Care and Social Reproduction

- Operational definition: childcare, eldercare, disability support, family support, and unpaid care labor are core infrastructure.
- Mechanisms: paid family leave; universal childcare access; dignified eldercare; disability-rights enforcement; recognition of unpaid care work in income, time, and pension systems.
- Bound by: VAL-001 (rights); VAL-002 (health); VAL-012 (mental health).
- Primary indicators: care-access metrics; caregiver-burden distribution; child-welfare metrics; elder-isolation rate; disability-inclusion audits.
- Measurement caveat: care work is feminized in most contexts; gender-disaggregated measurement required.

### VAL-018 Continuous Self-Correction

- Operational definition: the society contains feedback loops, adversarial review, amendment procedures, and peaceful reform mechanisms.
- Mechanisms: standing adversarial-review body; periodic constitutional convention; whistleblower channels; protected dissent; sunset clauses on rules.
- Bound by: VAL-005 (legitimacy of reform); VAL-006 (capture resistance of reform processes).
- Primary indicators: amendment throughput; contradiction-resolution time; audit-response rate; reform-participation rate.
- Measurement caveat: too much amendment churn is destabilizing; too little is sclerotic.

### VAL-019 Internal Observability and Secure Boundaries

- Operational definition: government, public institutions, and society-scale processes are observable and auditable by members; private life is protected; external interfaces have explicit security boundaries.
- Mechanisms: public decision logs; institutional metrics dashboards; audit-trail access; cryptographic separation of public and personal data; explicit external-boundary policy (physical, cyber, info, economic, biosecurity).
- Bound by: VAL-001 (rights); VAL-006 (capture resistance); VAL-015 (privacy); VAL-018 (self-correction).
- Primary indicators: public-audit coverage; decision-log completeness; member-access latency; external-boundary breach rate.
- Measurement caveat: this is the value most prone to mission creep into surveillance; constant vigilance required.

## Article III: Value Conflicts and Tradeoff Zones

This article specifies how the framework handles known recurring conflicts among values. These are not "resolved" in the abstract; the constitution states procedure and weighting for cases.

### TZ-001 Liberty vs. Security (VAL-001 vs. VAL-004 / VAL-019)

- Rule: in non-crisis conditions, rights default to permissive; restrictions require legal authority, proportionality, and judicial review.
- In crisis: emergency restrictions are time-limited (default 30 days, renewable only with supermajority and judicial review), narrowly tailored, reported publicly, and automatically expire absent reauthorization.
- Non-derogable: VAL-001 non-derogable elements stand in all crises.

### TZ-002 Pluralism vs. Anti-Pluralism (VAL-010 vs. movements seeking supremacy)

- Rule: pluralism is protected; institutions enforce non-discrimination law and equal access; suppression of belief or speech is constrained by VAL-001 and VAL-008.
- The framework rejects "tolerance of intolerance" as a paradox by distinguishing belief (protected) from conduct that violates others' rights (regulated under law).

### TZ-003 Self-Correction vs. Stability (VAL-018 vs. VAL-004)

- Rule: amendment procedures are explicit, accessible, and predictable; thresholds vary by impact (operational rules: simple legislative; constitutional: supermajority + time delay + ratification).
- Periodic constitutional review (every 20-25 years) is mandatory to prevent sclerosis.

### TZ-004 Transparency vs. Privacy (VAL-019 vs. VAL-015)

- Rule: institutions are observable; individuals are not. Data about institutions (decisions, budgets, performance) is public by default; data about individuals is private by default.
- Member-level data may be aggregated for institutional accountability; raw personal data may not be released without consent or court order.
- "Public figures" exception applies to office-related conduct only.

### TZ-005 Competence vs. Democratic Legitimacy (VAL-007 vs. VAL-005)

- Rule: competence-gating exists for technical roles (judges, central bankers, regulators, doctors); democratic legitimacy for direction-setting; sortition and deliberation for value-loaded contested questions.
- Competence assessment must be transparent and contestable to avoid credentialism (VAL-006).

### TZ-006 Local Autonomy vs. Universal Rights (subsidiarity vs. VAL-001)

- Rule: local communities have substantial autonomy over their own affairs; universal rights apply to all members regardless of locality.
- Local rules that conflict with universal rights yield to universal rights, enforced by national courts.

### TZ-007 Present Wellbeing vs. Future Generations (current members vs. VAL-016)

- Rule: future-generations advocate has consultative status in major decisions; quantitative long-horizon impact statements are required; ecological boundaries (VAL-003) are binding.
- Present members may decide on intra-generational consumption tradeoffs but may not deplete the resource base or transfer unsustainable debt to future generations.

### TZ-008 Care Burden vs. Autonomy (VAL-017 vs. VAL-001)

- Rule: care work is recognized economically and politically; care relations are voluntary at adult level (no forced caregiving); state provides infrastructure so that caregivers are not coerced by absence of alternatives.

### TZ-009 Member Observability vs. Whistleblower Safety (VAL-019 vs. VAL-001 / VAL-018)

- Rule: member observability covers institutional decisions, processes, and aggregated outcomes; identities of whistleblowers, informants, and individuals reporting abuse are protected.
- Reporters of crime are protected as a special case under VAL-008.

### TZ-010 Economic Innovation vs. Concentration (VAL-014 vs. VAL-006)

- Rule: market activity is permitted and supported; concentrations of economic power that translate into political power are structurally limited by antitrust, taxation, and political-finance rules.

## Article IV: Conflict Resolution Procedure

When values conflict in a specific case:

1. The deciding body identifies the affected value IDs.
2. The body describes the conflict in concrete institutional terms.
3. The body proposes at least two resolution options.
4. The body states who bears the cost of each option.
5. The body identifies what evidence or simulation would favor one option.
6. The body records the decision in the decision log (ART-027) with reasoning.
7. If resolution requires constitutional interpretation, the matter is referred to the constitutional review body before final decision.

## Article V: Amendment Procedure

Constitutional amendments require:

1. A named change proposal with a stable ID.
2. A rationale grounded in evidence, contradiction resolution, or simulation results.
3. A compatibility analysis against all existing values.
4. An adversarial review from at least three perspectives: skeptic, historian, behavioral scientist.
5. A migration note explaining what existing artifacts must change if accepted.
6. A public deliberation period of at least 90 days.
7. Adoption by supermajority of representative body and ratification by citizen referendum or sortition assembly, depending on amendment scope.

Non-amendable provisions: VAL-001 non-derogable elements; the amendment procedure itself; the prohibition on becoming a one-party state; the prohibition on hereditary office.

## Article VI: Binding Interpretation

Where this constitution and any other artifact in this iteration conflict, this constitution governs.

Where this constitution and `canon/values.md` conflict, the canon governs and this artifact must be revised.

Where two values in this constitution conflict in a specific case, the conflict-resolution procedure (Article IV) applies, and the resulting interpretation enters the decision log as precedent.

## Article VII: Reservations and Open Questions

This baseline constitution has the following acknowledged open questions, to be resolved in future iterations:

- Exact thresholds for emergency-power renewal (TZ-001) are not specified; module ART-017 will propose them.
- Boundary between competence-gated and democratic roles (TZ-005) requires case-by-case design in ART-009.
- Operationalization of future-generations representation (TZ-007 / VAL-016) is in ART-009 and ART-015.
- The framework's interaction with non-member residents (visitors, asylum seekers, stateless people) is partially specified here under VAL-001 and elaborated in ART-011 and ART-017; further detail is needed.
- The relationship to non-human persons (great apes, cetaceans, AI systems) is deferred to a future iteration.
