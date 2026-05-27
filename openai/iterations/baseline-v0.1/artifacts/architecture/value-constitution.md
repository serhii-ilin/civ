# Value Constitution

Iteration: `baseline-v0.1`

Status: `draft`

Source of truth: `canon/values.md`

## Constitutional Values

This artifact adopts `VAL-001` through `VAL-019` from the canon without amendment. The baseline design treats the values as binding constraints, not aspirational branding.

| ID | Value | Definition | Example Indicators |
| --- | --- | --- | --- |
| VAL-001 | Human Dignity and Rights | Every person has inherent worth, bodily autonomy, due process, freedom of conscience, freedom of association, and protection from arbitrary coercion. | Civil liberties index, due-process access, rights-violation rate, minority-rights protections |
| VAL-002 | Health by Design | Physical, mental, relational, and societal health are structural design goals, not downstream aspirations. | Life expectancy, healthy life years, preventable disease burden, loneliness index, family stability |
| VAL-003 | Ecological Boundaries | Economic, industrial, and social systems must operate within planetary and local ecological limits. | Material footprint, carbon budget, biodiversity impact, water stress, land-use intensity |
| VAL-004 | Resilience as Architecture | The society must survive, adapt, and recover from ecological, economic, military, technological, institutional, and cultural shocks. | Recovery time, reserve capacity, redundancy, supply-chain dependency, institutional continuity |
| VAL-005 | Legitimate and Consent-Based Governance | Governance must be competent and also perceived as fair, contestable, and consent-based by the governed. | Trust in institutions, participation rates, appeal success rates, perceived procedural fairness |
| VAL-006 | Capture-Resistant Governance | Power concentration, nepotism, corruption, regulatory capture, and institutional capture must be structurally constrained. | Power concentration metrics, conflict-of-interest findings, lobbying transparency, enforcement independence |
| VAL-007 | Competence with Accountability | Roles with public authority require verified competence, ethical fitness, transparent review, and removal mechanisms. | Qualification validity, performance audits, recall/removal rates, error correction time |
| VAL-008 | Justice and Rule of Law | Law must be public, consistent, rights-protecting, proportionate, reviewable, and accessible to all. | Legal access, case duration, wrongful conviction rate, police abuse rate, restorative resolution rate |
| VAL-009 | Science-Guided Policy | Empirical questions should be answered through evidence and transparent uncertainty, while moral tradeoffs remain democratically and constitutionally governed. | Evidence grading compliance, replication status, policy review cadence, uncertainty disclosure |
| VAL-010 | Pluralism and Freedom of Conscience | The society must protect religious, spiritual, philosophical, cultural, and lifestyle diversity without granting any group institutional supremacy. | Viewpoint diversity, discrimination rates, exit rights, cultural participation |
| VAL-011 | Education as Foundation | Education develops cognitive resilience, emotional intelligence, practical skill, civic literacy, and lifelong learning capacity. | Literacy, numeracy, critical-thinking assessment, civic knowledge, adult reskilling access |
| VAL-012 | Mental Health as Civic Infrastructure | Psychological wellbeing is a public infrastructure concern, not only an individual healthcare responsibility. | Access to care, suicide rate, trauma exposure, social support density, treatment wait time |
| VAL-013 | Self-Sufficiency and Chosen Interdependence | Individuals, families, communities, and larger systems should be capable of basic independent function while benefiting from voluntary interdependence. | Local production floors, household preparedness, community reserve duration, dependency concentration |
| VAL-014 | Sustainable Progress Beyond GDP | Growth must be redefined as measurable improvement in wellbeing, capability, resilience, justice, and ecological balance. | Genuine progress indicators, wellbeing indices, inequality, ecological drawdown, innovation quality |
| VAL-015 | Privacy and Data Rights | Transparency for institutions must not become surveillance of people; data collection requires purpose limitation, consent, minimization, and auditability. | Data breach rate, surveillance warrant rate, consent compliance, algorithmic audit results |
| VAL-016 | Intergenerational Stewardship | Decisions must protect the rights, resources, institutions, and ecological base of future generations. | Long-term debt, ecological debt, infrastructure maintenance, youth wellbeing, future-risk exposure |
| VAL-017 | Care and Social Reproduction | Childcare, eldercare, disability support, family support, and unpaid care labor are core infrastructure. | Care access, caregiver burden, child welfare, elder isolation, disability inclusion |
| VAL-018 | Continuous Self-Correction | The society must contain feedback loops, adversarial review, amendment procedures, and peaceful reform mechanisms. | Amendment throughput, contradiction resolution time, audit response rate, reform participation |
| VAL-019 | Internal Observability and Secure Boundaries | Government, public institutions, and society-scale processes must be observable and auditable by members, while private life is protected and external interfaces have explicit security boundaries. | Public audit coverage, decision-log completeness, member observability access, observability latency, external boundary breach rate, cyber and physical access-control audits |

## Operational Interpretation

| Value Cluster | Values | Baseline Interpretation |
| --- | --- | --- |
| Rights and legality | VAL-001, VAL-008, VAL-010, VAL-015 | Individual rights, due process, dissent, association, conscience, and privacy set hard limits on institutional design. |
| Health and care | VAL-002, VAL-012, VAL-017 | Health, mental health, childhood, eldercare, disability support, and caregiving are core infrastructure. |
| Ecology and resilience | VAL-003, VAL-004, VAL-013, VAL-016 | Ecological ceilings, redundancy, local production floors, and future-generation duties constrain economic and infrastructure choices. |
| Legitimate competence | VAL-005, VAL-006, VAL-007, VAL-009, VAL-018 | Authority requires legitimacy, skill, evidence discipline, anti-capture design, review, and removal. |
| Sustainable progress | VAL-011, VAL-014, VAL-019 | Education, internal observability, and progress metrics must track capability, wellbeing, justice, ecology, and resilience rather than GDP alone. |

## Baseline Tradeoffs

| Tradeoff ID | Values in Tension | Baseline Rule | Review Trigger |
| --- | --- | --- | --- |
| VTR-001 | VAL-019 vs VAL-015 | Public institutions are observable by default; private persons are private by default. Exceptions require legal authorization, purpose limitation, and audit. | Data misuse, chilling effects, or unresolved security incidents. |
| VTR-002 | VAL-005 vs VAL-007 | Democratic legitimacy controls goals and removal; competence gates control access to specialized authority. | Competence gates show class, ideology, or credential capture. |
| VTR-003 | VAL-003 vs VAL-014 | Economic growth is acceptable only inside ecological caps and social-foundation guarantees. | Boundary breach, essential-service decline, or hidden ecological externalities. |
| VTR-004 | VAL-001 vs VAL-004 | Crisis measures may limit ordinary activity only under necessity, proportionality, expiration, remedy, and review. | Emergency renewal, rights complaints, or security secrecy expansion. |
| VTR-005 | VAL-010 vs VAL-013 | Communities may cultivate distinct cultures but must preserve exit rights, non-discrimination, and access to common rights. | Local exclusion, family coercion, or minority-rights violations. |

## Conflict-Resolution Rules

When values compete, the iteration must:

1. Identify the affected value IDs.
2. Describe the conflict in concrete institutional terms.
3. Propose at least two resolution options.
4. State who bears the cost of each option.
5. Define what evidence, stakeholder input, or simulation result would favor one option.
6. Record the choice in `review/decision-log.md` and unresolved issues in `review/contradiction-register.md`.

## Amendment Status

No amendments are proposed in `baseline-v0.1`. Open contradiction `CON-001` tracks the unresolved boundary between member observability and privacy.

## Amendment Rules

Future amendments require:

- A named change proposal with a stable ID.
- A rationale grounded in evidence, contradiction resolution, or simulation results.
- Compatibility analysis against all existing values.
- Adversarial review from skeptic, historian, and behavioral-scientist perspectives.
- A migration note identifying affected artifacts and transition risks.
