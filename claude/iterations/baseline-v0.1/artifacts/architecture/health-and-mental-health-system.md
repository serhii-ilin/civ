# Health and Mental Health System

Artifact ID: ART-012
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: MOD-HMH
Depends on: ART-008

## Purpose

Specify the health, public health, and mental health system as civic infrastructure. Bound by `value-constitution.md` (ART-008), behavioral findings in ART-007, and economic structure in ART-010.

Health is treated as a structural design output, not as a downstream consequence. The system is universal, anchored in primary care, locally networked, trauma-informed by default, and resistant to surveillance creep.

## Core Architecture (HEA-A)

### HEA-A1 Universal Coverage

- All members and lawful residents have unconditional access to a defined essential benefit package without point-of-service charges for essential care.
- Coverage continues regardless of employment, marital status, or location within the polity.
- Reflects LAW-R2.2 and VAL-002.

### HEA-A2 Tiered Delivery

- Tier 1 — Primary care, community clinics, school-based services, home visiting, public-health outreach.
- Tier 2 — Specialty outpatient, mental health teams, day surgery, community hospitals.
- Tier 3 — Tertiary hospitals, complex specialty, transplant, advanced critical care.
- Tier 4 — Quaternary centers for rare and complex conditions; research-integrated.

### HEA-A3 Primary Care Anchoring

- Every member has a registered primary-care team (physician or nurse practitioner, with nursing, social work, mental-health, pharmacy support).
- Primary care is the default entry point; specialist access is by referral with patient-controlled exceptions.
- Continuity of care prioritized; assignment stable absent member request to change.

### HEA-A4 Locally Networked Care

- Care is organized around catchment areas of approximately 50,000 to 200,000 people, mapped to regional governance.
- Local health councils include clinicians, public health, social work, community representatives, and patient advocates.

### HEA-A5 Public Insurance and Provider Mix

- Single public payer at national tier; regional administration.
- Provider mix is plural: public hospitals, not-for-profit hospitals, regulated for-profit providers in specific markets, cooperative clinics.
- For-profit provision is permitted in tiers and services where it does not threaten access or quality; profit margins are regulated.

## Mental Health (HEA-M)

### HEA-M1 Mental Health as Civic Infrastructure

- Mental health is treated structurally: built environment (HEA-M5), community (ART-014), economy (ART-010), education (ART-013), and justice (ART-011) systems share responsibility.
- Service access is universal and on parity with physical health under HEA-A1.

### HEA-M2 Service Layers

- Layer 1: Universal prevention — school, workplace, community mental-health education; destigmatization; peer-support infrastructure.
- Layer 2: Early intervention — accessible counseling, brief therapy, crisis lines, walk-in mental-health centers.
- Layer 3: Specialty care — outpatient psychiatry, psychology, allied therapies, addiction treatment, trauma-specialty care.
- Layer 4: Acute and intensive — crisis-stabilization units, inpatient psychiatry with rights protections, intensive case management, assertive community treatment.

### HEA-M3 Crisis Response

- Mental-health crisis calls are routed to specialized civilian responders, not police, except where there is imminent violence (per LAW-P2).
- Crisis-stabilization is the default; involuntary admission requires judicial process with prompt review (LAW-P5).
- Crisis lines are toll-free, multilingual, available 24/7 with both phone and text.

### HEA-M4 Trauma-Informed Default

- All clinical services use trauma-informed practice as default (B-008, B-009, CLM-043).
- Public institutions (schools, courts, social services, immigration) train staff in trauma awareness.

### HEA-M5 Built Environment for Mental Health

- Anti-isolation design embedded in zoning and infrastructure (ART-015): walkable neighborhoods, public spaces, mixed-use density.
- Mental-health impact assessments for major infrastructure decisions.

### HEA-M6 Substance Use

- Substance-use is treated as a health issue, not criminal.
- Decriminalization of personal possession of currently illegal substances paired with regulated access pathways and substantial investment in treatment.
- Harm-reduction services (supervised consumption, drug checking, opioid agonist therapy, naloxone distribution).
- Tobacco, alcohol, cannabis, and other regulated substances subject to public-health-based regulation: minimum age, advertising restrictions, taxation, retail density limits.

### HEA-M7 Specific Populations

- Children and adolescents: school-based mental health, family support, juvenile-justice mental-health screening.
- Older adults: depression screening, isolation prevention, dementia care.
- People with severe mental illness: long-term assertive community treatment, housing-first approach, family support.
- People with intellectual and developmental disabilities: lifelong support, family respite, community-living infrastructure.
- People in custody: equal access to mental health, prohibition on punitive isolation of those with mental illness (LAW-P5).

## Public Health (HEA-P)

### HEA-P1 Surveillance and Privacy

- Disease surveillance uses minimum necessary data; aggregated reporting by default; identifiable data only with specific justification and time limits.
- Strict separation between public-health surveillance and law enforcement; data flows between agencies controlled by statute.
- Mandatory reporting limited to defined conditions (communicable disease, certain injuries).
- See ART-016.

### HEA-P2 Communicable Disease

- Vaccination access universal; vaccine schedules updated regularly; school and workplace policies set by public-health authority.
- Outbreak response coordinated nationally with regional implementation; preparedness plans rehearsed annually.
- Antimicrobial stewardship.

### HEA-P3 Pandemic Preparedness

- Standing pandemic-preparedness body with budget; surge capacity; reserved manufacturing for vaccines, antivirals, PPE.
- Pre-authorized legal frameworks for emergency public-health measures with sunset clauses, judicial review, and non-derogable rights protection (LAW-R5, GOV-D5).
- International cooperation pathways pre-built (WHO IHR, cross-border partnerships).
- Communication infrastructure: public-interest broadcasting, social-platform partnerships under transparency requirements.

### HEA-P4 Environmental Health

- Air, water, soil, noise, radiation standards.
- Industrial-hazard regulation.
- Climate-related health: heat, wildfire smoke, flooding response, vector-borne disease.
- Built-environment standards for health (HEA-M5).

### HEA-P5 Food and Nutrition

- Food safety regulation.
- Nutrition labeling and food-marketing regulation, with strong restrictions on marketing to children.
- Public-school food programs of nutritional standard.
- See ART-015.

### HEA-P6 Maternal, Child, and Reproductive Health

- Free comprehensive maternal care; midwifery integrated; doula support.
- Free pediatric care; school health programs.
- Reproductive autonomy: contraception, abortion, fertility care, sterilization at member request.
- Bound by VAL-001 (bodily autonomy) and LAW-R1.

### HEA-P7 Occupational Health

- Workplace exposure standards.
- Mental-health protections at work.
- Hazardous-work regulation.

### HEA-P8 Health Emergencies

- Defined categories: pandemic, mass casualty, environmental, mental-health crisis.
- Pre-authorized response with sunset clauses (HEA-P3).
- Coordination with civil defense (ART-017).

## Health Information Infrastructure (HEA-D)

### HEA-D1 Personal Health Records

- Members hold authoritative copy of their health records with access at any time.
- Providers access via consent; emergency access logged; member control over sharing.

### HEA-D2 Public Health Data Commons

- De-identified aggregate health data are a public-research commons under strict privacy protections.
- Re-identification attempts criminal.
- Member opt-out from aggregate data possible but discouraged.

### HEA-D3 Clinical Decision Support

- AI-assisted clinical tools regulated under HEA-D3 and ART-016: risk-tiered, validated, transparent on limits, do not make autonomous high-stakes clinical decisions.

### HEA-D4 Research Ethics

- Research ethics boards mandatory for human-subjects research.
- Informed consent rigorous; participation always voluntary.
- Publication of all trials; pre-registration required for clinical trials.

## Workforce (HEA-W)

### HEA-W1 Provider Education and Distribution

- Public funding of medical, nursing, allied-health education with service obligations for underserved areas.
- Workforce planning to match population needs.
- Continuing education required.

### HEA-W2 Workforce Wellbeing

- Hours-of-work limits for clinical staff.
- Mental-health support for clinicians (occupational mental-health is acute risk in healthcare).
- Anti-burnout staffing standards.

### HEA-W3 Workforce Diversity

- Active recruitment from underrepresented communities.
- Cultural-competence training.

### HEA-W4 Allied Workforce

- Community health workers and peer-support workers as core workforce.
- Care workers (eldercare, disability support, child care) recognized and fairly compensated (VAL-017, ECO-W).

## Cost Control and Financing (HEA-F)

### HEA-F1 Financing

- Single payer at national level funded through general taxation and earmarked health-insurance contributions.
- Cross-subsidization across regions to equalize access.

### HEA-F2 Cost Control

- Tariff-setting by independent board with public reasoning.
- Bulk procurement of medicines, devices.
- Mandatory licensing for essential medicines (ECO-P4).
- Price transparency; international reference pricing.

### HEA-F3 Quality

- Independent quality regulator; public reporting of provider quality metrics with risk adjustment.
- Patient-safety reporting infrastructure; blame-free reporting protected; system-level learning.

## End of Life and Palliative Care (HEA-E)

- Palliative care accessible to all who need it.
- Advance directives respected.
- Medical assistance in dying: permitted under defined eligibility (terminal illness, intolerable suffering, capacity, voluntariness, safeguards); conscientious-objection protected.
- Bereavement support available.

## Indicators (HEA-I)

- Mortality: all-cause, condition-specific, maternal, infant.
- Morbidity: prevalence and incidence of priority conditions.
- Mental health: prevalence, treatment access, treatment retention, suicide rate, self-harm hospitalization.
- Loneliness and social connection.
- Substance use: prevalence, treatment access, overdose mortality.
- Access: wait times by service; geographic distribution; rejection rates.
- Equity: outcomes by demographic, region, income.
- Safety: adverse-event rates, never-event rates.
- Workforce: shortage indices, burnout, retention.
- Cost: per-capita health spending, share of GDP, OOP burden.
- Public health: vaccination coverage, outbreak response times, environmental-health-standard compliance.

Goodhart-Campbell caution (CLM-189): no single quality measure tied to provider pay in a way that incentivizes patient selection or measurement gaming; quality measurement is multi-dimensional and audited.

## Open Issues

- Mental-health workforce is in chronic shortage globally; the framework's universal-access promise requires large-scale workforce investment with multi-decade lead time.
- Drug pricing under mandatory licensing interacts with international IP regimes; transitional path needed (ART-024, ART-026).
- AI clinical decision support is evolving fast; framework regulation must remain adaptive (ART-016).
- End-of-life policy is morally contested; the framework's posture is permissive within safeguards, but cultural variation requires regional adaptation within constitutional limits.
- Surveillance vs. public-health-effectiveness tradeoff during pandemic response is unresolved at full satisfaction; the framework errs toward narrow data use with strong sunsets (HEA-P1).
- Climate-driven health threats (HEA-P4) will intensify; preparedness budget must scale.

## Cross-References

- Bound by: VAL-002, VAL-012, VAL-015, VAL-017.
- Coordinates with: ART-013 (education), ART-014 (community), ART-011 (law), ART-015 (ecology), ART-016 (technology).
- Tested in: pandemic scenarios, mental-health crisis scenarios, drug-pricing scenarios.
