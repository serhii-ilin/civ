# ART-012: Health and Mental Health System Architecture

Iteration: `baseline-v0.1`
Status: draft

## Purpose

Design health, public health, and mental health as civic infrastructure. The system must guarantee universal access, prevent illness through structural design, provide community-level early warning and support, and protect against coercive or surveillance-heavy health interventions.

## Core Design Principles

1. **Health is infrastructure, not consumption**: Health systems are public goods that enable all other social and economic function. They must be funded, designed, and maintained as infrastructure, not as a market commodity.
2. **Prevention over treatment**: Structural prevention (clean air, water, food, safe housing, walkable communities, trauma prevention) is the most cost-effective health investment.
3. **Integration of physical and mental health**: No separation of "medical" from "mental" -- every health interaction integrates both.
4. **Trauma-informed by default**: All health institutions are trauma-informed (BF-007): safety, trustworthiness, peer support, collaboration, empowerment, cultural responsiveness.
5. **No coercion, no surveillance on suspicion**: Public health and mental health interventions must be consent-based except where imminent danger to self or others meets strict legal criteria (see emergency provisions).
6. **Community-embedded, not centralized**: Healthcare is organized at community and regional scales with national standards, not national command.

## System Architecture: Three Tiers

### Tier 1: Community Health Network

The foundation of the system, embedded in every community cell (100-300 people).

**Components**:
- **Community Health Coordinator**: Full-time health professional (nurse practitioner or equivalent) living in the community. 1 per 300 people. First point of contact for health concerns.
- **Community Mental Health Facilitator**: Mental health professional providing counseling, crisis intervention, group therapy, and mental health literacy. 1 per 500-1000 people.
- **Community Care Network**: Volunteers and trained community members providing daily-living support, companionship, medication reminders, transport, and wellness checks. Coordinated by Community Health Coordinator.
- **Health Space**: Community clinic with consultation rooms, telemedicine station, basic diagnostics, and meeting space for health education and support groups.

**Functions**:
- Primary care and preventive services
- Chronic disease monitoring
- Maternal and child health
- Mental health counseling and group therapy
- Addiction support and harm reduction
- Health literacy and education
- Social-prescribing (connecting people to community resources)
- Early warning: identification of isolation, deterioration, family stress, child welfare concerns
- End-of-life and palliative care at home
- Referral and navigation to higher tiers

### Tier 2: Regional Health System

Serves clusters of communities (50,000-200,000 population).

**Components**:
- **Community Hospital**: Local hospital with emergency department, inpatient beds, surgery, obstetrics, mental health inpatient unit, diagnostic imaging, laboratory. Sized for 50,000-200,000 population.
- **Specialist Clinics**: Rotating specialists (cardiology, endocrinology, orthopedics, psychiatry, pediatrics, etc.) serving multiple community hospitals.
- **Regional Public Health Unit**: Epidemiology, disease surveillance, environmental health, health promotion, outbreak investigation and response.
- **Regional Mental Health Center**: Inpatient and outpatient mental health services, addiction treatment, crisis stabilization, children's mental health, trauma recovery programs.
- **Regional Emergency Medical Services**: Ambulance and emergency transport, coordinated with community first responders.

### Tier 3: National Health Infrastructure

**Components**:
- **National Health Service (NHS-mandate)**: Single-payer, publicly funded, universally accessible. All healthcare free at point of use.
- **National Public Health Agency**: Independent scientific agency (parallel to central-bank independence). Pandemic preparedness, disease surveillance, health-data analysis, health-impact assessment of policies, health-inequality monitoring. Director appointed for 10-year non-renewable term; budget indexed to population health indicators.
- **National Institute for Health and Care Excellence (NICE-model)**: Independent evidence-evaluation body determining clinical effectiveness and cost-effectiveness of treatments, technologies, and public-health interventions. Determines what the NHS covers based on evidence, not politics.
- **Health Technology Assessment Agency**: Evaluates new health technologies and pharmaceuticals for safety, efficacy, and cost-effectiveness before adoption.
- **Health Data Infrastructure**: Interoperable electronic health records (patient-controlled), population-health analytics (anonymized), health-system performance metrics (publicly visible).
- **Strategic Medical Reserve**: National stockpile of essential medicines, vaccines, PPE, ventilators, and emergency supplies for 6-month pandemic/disaster scenario.

---

## Mental Health: Deep Design

### Tiered Access Model

| Level | Service | Access Model |
| --- | --- | --- |
| Universal | Mental health literacy education (MOD-EDU); community mental health awareness; stress-management tools; mindfulness resources; peer support networks | Available to all, no referral |
| Primary | Community Mental Health Facilitator; group therapy; brief counseling (6-12 sessions); digital mental health tools; social prescribing | Self-referral or Community Health Coordinator referral; no wait >2 weeks |
| Secondary | Specialist psychotherapy (CBT, DBT, EMDR, etc.); psychiatric consultation; addiction treatment programs; trauma therapy | Primary referral; no wait >4 weeks |
| Tertiary | Inpatient psychiatric care; crisis stabilization; intensive outpatient; long-term psychiatric disability support | Secondary referral or emergency admission |
| Crisis | 24/7 crisis line; mobile crisis teams (mental health professionals, not police); crisis stabilization units (alternative to ER); peer respite houses | Immediate access, no referral |

### Design Features

- **No police as mental-health crisis responders**: Mobile crisis teams consist of mental health professionals, peer support workers, and paramedics. Police involved only when credible threat of violence exists.
- **Crisis stabilization, not emergency-room boarding**: Dedicated crisis-stabilization units with calm environment, peer support, and immediate therapeutic engagement. Average stay 24-72 hours.
- **Peer support integration**: Trained peer-support workers (people with lived experience of mental health conditions) integrated at all levels as paid professionals.
- **Family and community support**: Family psychoeducation, support groups, and respite services as standard care components.
- **Prevention through structure**: Built environment (walkable, green, third places -- CLM-023); economic security (CLM-006); social connection (BF-005); trauma-informed institutions (CLM-016); ACE prevention (CLM-009).

---

## Public Health Infrastructure

### Surveillance and Early Warning
- **Wastewater monitoring**: Pathogen, drug, and chemical surveillance at community level. Privacy-protective population-level data.
- **Syndromic surveillance**: Real-time monitoring of emergency-department visits, pharmacy dispensing, school/work absence, and telehealth queries.
- **Genomic surveillance**: Pathogen sequencing for outbreak tracking and variant identification.
- **Sentinel physician networks**: Community Health Coordinators reporting unusual presentations.
- **Environmental monitoring**: Air quality, water quality, vector surveillance, climate-health indicators.
- **Health-equity monitoring**: Real-time tracking of health outcomes by socioeconomic, geographic, and demographic variables to detect emerging disparities.

### Pandemic and Health Emergency Architecture

**Declaration**: National Public Health Agency Director, in consultation with National Executive, declares public health emergency. Emergency must be confirmed or terminated by National Assembly within 14 days.

**Powers**:
- Travel restrictions and quarantine (with due process: appeal, humane conditions, compensation for lost income).
- Mandatory vaccination with medical exemption only -- IF and ONLY IF: (a) disease is severe (mortality >1% or severe long-term disability), (b) highly transmissible (R0 > 2), (c) vaccine is proven safe and effective through Phase 3 trials, risk of vaccination is less than risk of disease for all demographic groups, and all NICE-model public-health criteria for mandatory-interventions thresholds are met, and (d) voluntary uptake is insufficient to achieve herd immunity after adequate public education and access period. This is an extreme measure, not a routine one, and must meet ALL criteria.
- Public-gathering restrictions (tiered by risk, with economic support for affected businesses and workers).
- Healthcare-worker emergency redeployment (with hazard pay, mental-health support, and voluntary opt-out for high-risk individuals).
- Temporary health-data sharing for pandemic response (time-limited, purpose-specified, with independent oversight).

**Limitations** (per VAL-002 health safeguards and VAL-001 bodily autonomy):
- Health interventions require informed consent except:
  - Imminent danger to self or others (mental health involuntary assessment, time-limited with judicial review)
  - Public health emergency as defined above
  - Incompetent patients without advance directives (temporary treatment to stabilize, with rapid guardianship/advance-directive resolution)
- Lockdowns of healthy/asymptomatic people are measures of last resort.
- Health-surveillance data may not be used for non-health purposes (law enforcement, employment, insurance).
- Emergency powers expire automatically after 90 days unless renewed by National Assembly with updated evidence of necessity.
- Post-emergency mandatory review: National Public Health Agency publishes comprehensive review within 60 days.

---

## Family, Trauma, Addiction, and Disability Support

### Family Systems Support
- **Universal home visiting**: All families with newborns receive home visits from community health worker (first 2 years). Intensity varies by assessed need. Non-punitive, supportive.
- **Parenting support**: Evidence-based parenting programs (Triple P, Incredible Years, etc.) universally available.
- **Family therapy**: Accessible through primary mental health services.
- **Child protection**: Mandated reporting with multi-disciplinary response (social work + health + education + legal). Emphasis on family preservation where safe; removal and foster care as last resort. Kinship care preference.
- **Domestic violence**: Integrated health-justice-community response. Safe housing, legal protection, counseling, economic support. Perpetrator programs.

### Trauma Recovery Infrastructure
- **Universal trauma screening**: ACE screening in primary care, schools, and community health settings (opt-in, not mandatory). Followed by supported referral to trauma services.
- **Trauma recovery programs**: Evidence-based trauma therapies (EMDR, TF-CBT, prolonged exposure, somatic experiencing, etc.) available at all Regional Mental Health Centers.
- **Trauma-informed training**: Mandatory for all health, education, justice, and social-service professionals.
- **Community trauma response**: Teams deployable after community traumatic events (violence, disaster, accident) for psychological first aid and ongoing support.

### Addiction and Substance Use
- **Harm reduction**: Needle exchange, supervised consumption sites, naloxone distribution, drug checking.
- **Treatment on demand**: No waitlists for addiction treatment. Medication-assisted treatment (methadone, buprenorphine) immediately accessible.
- **Decriminalization of personal possession**: Drug use treated as health issue, not criminal issue. Possession for personal use decriminalized. Trafficking and production remain illegal.
- **Social determinants**: Housing First model (housing + wraparound support without preconditions of sobriety); employment support; community reintegration.

### Disability and Aging Support
- **Universal design**: Public spaces, transportation, housing, and digital services designed for accessibility from outset, not retrofitted.
- **Independent living support**: Personal care assistance, home modification, assistive technology, community support workers -- sufficient to enable independent living at community standard.
- **Disability income support**: Sufficient for dignified living above poverty line, without forcing poverty through means-testing.
- **Aging in community**: Intergenerational housing, aging-in-place support, elder community centers, elder cohousing options.
- **Caregiver support**: Respite care, caregiver training, caregiver mental-health support, caregiver financial compensation.
- **Dementia care**: Specialized support, safe environments, caregiver support, community awareness and inclusion.

---

## Observability

All health-system data publicly accessible (anonymized, aggregated) including:
- Wait times by service, geography, and demographic
- Health outcomes by geography and demographic (disparity detection)
- Mental health access and outcomes
- Public health indicators (real-time dashboard)
- Health-system financial transparency
- Patient satisfaction and experience
- Health-impact assessments of major policies
- Public health emergency justifications and evidence

Individual patient data strictly protected. Health data not accessible to law enforcement, immigration, employers, or insurers without explicit patient consent or court order meeting strict necessity criteria.

**Decision**: DEC-HMH-001 (health-system model). Rationale: Universal single-payer system with community-embedded primary care, as evidence shows better outcomes at lower cost (CLM-022). Community health network integrates physical and mental health and closes the gap between clinical care and social determinants.

---

## Evidence and Assumptions

| Assumption ID | Statement | Test Method | Failure Signal |
| --- | --- | --- | --- |
| ASM-HMH-001 | Community Health Coordinator model achieves health outcomes at parity or better than physician-centered primary care for preventive and chronic care | Comparative outcome studies in pilot communities | Preventable hospitalizations or chronic-disease outcomes worse vs. traditional model |
| ASM-HMH-002 | Harm-reduction and decriminalization of personal possession reduces drug-related deaths and improves treatment engagement | Public health data; comparison with criminalized jurisdictions | Drug-related deaths increase after adjustment for trends |
| ASM-HMH-003 | Mobile crisis teams (non-police) reduce use of force and improve mental health outcomes vs. police-only mental health response | Comparative incident data; follow-up outcomes | Force incidents equal or higher; outcomes worse |

## Decision Log: Health

| Decision ID | Scope | Decision | Rationale | Evidence |
| --- | --- | --- | --- | --- |
| DEC-HMH-001 | Health-system model | Universal single-payer, community-embedded primary care, integrated physical/mental health | CLM-022: universal systems better outcomes at lower cost. Community embedding addresses social determinants. Integration prevents mental/physical siloing. | SRC-013, SRC-018, BCM-005 |
| DEC-HMH-002 | Mental health crisis response | Non-police mobile crisis teams as default | Evidence shows police involvement in mental health crises increases use of force, trauma, and criminalization without improving outcomes. Dedicated mental health crisis response is safer and more effective. | SRC-018 |
| DEC-HMH-003 | Substance use policy | Harm reduction + decriminalization of personal possession + treatment on demand | Evidence from Portugal, Switzerland, Netherlands, and others shows decriminalization + treatment reduces deaths, HIV/hepatitis transmission, and crime without increasing use rates. | SRC-018, European Monitoring Centre for Drugs |
| DEC-HMH-004 | Pandemic power limits | Strict criteria for mandatory measures; independent public-health agency; automatic expiration; post-emergency review | RSK-014 (emergency powers creep). VAL-002 safeguards against coercive health measures. VAL-001 bodily autonomy. Balance pandemic response with rights protection. | SRC-019, RSK-014 |

## Cross-Module Interfaces

| Interface | Partner Module | Requirement |
| --- | --- | --- |
| Governance | MOD-GOV | Public Health Agency independence; health-governance interface; emergency-powers limits |
| Law | MOD-LAW | Mental-health-justice interface; involuntary-treatment legal framework; drug-decriminalization; health-data privacy law |
| Community | MOD-CUL | Community care networks; social isolation prevention; community trauma response |
| Ecology | MOD-ECOINF | Healthy-built-environment standards; environmental-health monitoring; food-system-health interface |
| Education | MOD-EDU | School-health services; mental health literacy; trauma-informed education; ACE prevention |
| Economy | MOD-ECO | Healthcare funding; universal-services design; disability income support; care economy |