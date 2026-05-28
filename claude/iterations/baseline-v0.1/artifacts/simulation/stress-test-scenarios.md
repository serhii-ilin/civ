# Stress Test Scenarios

Artifact ID: ART-021
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: MOD-SIM
Depends on: ART-006, ART-018

## Purpose

Specify the stress scenarios that the framework must survive. Each scenario references one or more failure modes from `failure-mode-register.md` and one or more architecture subsystems from `technical-architecture.md`. Each scenario specifies: triggering conditions, intensity profile, expected dynamics, indicators to monitor, red lines that constitute framework failure, and adaptation criteria that indicate successful response.

These scenarios are designed for the hybrid modeling approach in `simulation-blueprint.md` (ART-019). Not every scenario requires every model type.

## Scenario Inventory

### SCN-001 Inequality-Power Feedback

- Covers: RSK-001, RSK-015, RSK-024.
- Setup: gradual increase in wealth concentration over 20 years; political-finance pressure intensifies.
- Variations: (a) baseline anti-capture mechanisms active; (b) mechanisms weakened by 50%; (c) mechanisms strengthened by 50%.
- Indicators: Gini, top-decile and top-percentile wealth share, political-finance disclosure adequacy, anti-trust enforcement actions, regulator-staff revolving-door rate, trust in institutions.
- Red lines: top-percentile wealth share crosses 30% sustained; lobbying-meeting density crosses threshold; sortition body abolished by capture.
- Adaptation criteria: structural anti-capture mechanisms (GOV-A) hold; wealth tax (ECO-T2) and antitrust (ECO-MK1) actions persist; sortition body retains independence; member observability functions.

### SCN-002 Demagogue Ascent

- Covers: RSK-002, RSK-019, RSK-022, RSK-035.
- Setup: economic shock plus information disorder; populist actor wins executive office or significant parliamentary share.
- Variations: (a) judicial independence intact; (b) two of three independent regulators captured; (c) emergency declared; (d) public-service media protected vs. weakened.
- Indicators: judicial independence index; election-administration integrity; press-freedom indicators; emergency-power scope and duration; opposition-suppression incidents; minority-rights audits.
- Red lines: constitutional court packed or coerced; election administration captured; political opposition imprisoned without due process; emergency powers extended beyond GOV-D5 limits without supermajority.
- Adaptation criteria: GOV-B5 functions; GOV-B3 maintains constitutional review; emergency expires; institutions hold.

### SCN-003 Fiscal Shock

- Covers: RSK-004, RSK-015, RSK-025.
- Setup: severe revenue shock (recession of 8% GDP plus capital flight); fiscal-rule pressure.
- Variations: tax instruments fixed vs. adaptive; sovereign wealth fund available vs. not; international support vs. isolation.
- Indicators: budget-deficit trajectory; sovereign-debt yield; banking-system buffers; UBI floor preservation; service-cut distribution.
- Red lines: UBI floor breached; banking-system insolvency; service-cut concentrated on vulnerable groups; sovereign default.
- Adaptation criteria: floor preserved; cuts distributionally fair; recovery within 5 years; tax-base reform passes.

### SCN-004 Cleavage Escalation

- Covers: RSK-005, RSK-017, RSK-018, RSK-038.
- Setup: identity-based political cleavage intensifies; violence localized.
- Variations: media architecture (recommender-driven vs. public-service); conflict-resolution capacity vs. none; truth-and-reconciliation history (recent vs. absent).
- Indicators: hate-crime rate; segregation indices; cross-cutting-association rate; security-service complaint distribution by group; conflict-resolution case volume.
- Red lines: hate-crime sustained increase >50% baseline; paramilitarization; security forces over-represented from one group; pluralism rights eroded.
- Adaptation criteria: enforcement non-discriminatory; minority rights protected; cross-cutting institutions maintained; conflict-resolution scaling.

### SCN-005 Climate Cascade

- Covers: RSK-006, RSK-012, RSK-039.
- Setup: severe regional drought, two consecutive harvest failures, sea-level event, climate-driven migration influx.
- Variations: ecological reserves vs. depleted; energy transition state; alliance support vs. isolation.
- Indicators: food security, water stress, biodiversity intactness, emergency-aid coverage, migration-reception capacity, energy reliability.
- Red lines: food insecurity exceeds 5% sustained; water rationing extended beyond 6 months; mass displacement uncontained.
- Adaptation criteria: ecological caps held; migration-reception capacity scaled; just-transition supported; long-horizon trajectory toward limits maintained.

### SCN-006 Pandemic

- Covers: RSK-007, RSK-013, RSK-027.
- Setup: novel respiratory pathogen with R0 ~ 2.5, IFR 1%; 18-month wave; vaccine development possible.
- Variations: preparedness investment levels; trust in public health; international coordination.
- Indicators: excess mortality, hospital capacity utilization, mental-health indicators, school-closure days, economic activity, surveillance-vs-privacy balance.
- Red lines: excess mortality >0.5% of population; healthcare system collapse; emergency-power retention beyond pandemic.
- Adaptation criteria: surge capacity holds; vaccine deployment equitable; mental-health support delivered; emergency powers expire on time; civil-liberties floor preserved.

### SCN-007 Cyber Critical-Infrastructure Attack

- Covers: RSK-008, RSK-033.
- Setup: coordinated attack on power, water, financial-system, communications; partial success.
- Variations: redundancy levels; air-gapping discipline; international support; insider co-conspirator vs. external only.
- Indicators: service-outage duration; cascading-failure spread; financial-system stability; communication integrity; public-trust during outage.
- Red lines: outage exceeds reserve durations (ART-015 ECN-IC2); financial-system insolvency; coordinated communication blackout.
- Adaptation criteria: critical services restored within targets; financial-system stabilizes; communication channels persist; attribution and response measured.

### SCN-008 AI-Information Shock

- Covers: RSK-009, RSK-010, RSK-020, RSK-042.
- Setup: capable generative-AI system used adversarially in election cycle; deepfakes at scale; recommender amplification; potential foreign coordination.
- Variations: TAI-R enforcement strength; public-service media integrity; civic literacy levels; international coordination.
- Indicators: detected synthetic-media share of political content; trust in election integrity; voter participation; rights-violation reports linked to AI; algorithmic-audit findings.
- Red lines: election integrity breached; mass-targeted manipulation undetected for >1 cycle; AI safety regulator captured.
- Adaptation criteria: detection and disclosure operational; election integrity preserved; TAI-A1 functions; rights protected.

### SCN-009 Foreign Invasion

- Covers: RSK-011, RSK-029.
- Setup: state-level military attack from neighbor; partial occupation possible.
- Variations: alliances; civil-defense readiness; energy and food sovereignty levels; legitimacy of government during war.
- Indicators: territorial integrity, civilian casualties, displacement, energy and food security, civil-liberties under emergency.
- Red lines: capitulation; war crimes by own forces; emergency-power abuse; loss of strategic resources.
- Adaptation criteria: defense effective within doctrine; civilian protection maintained; civil-liberties floor preserved; international law respected.

### SCN-010 Demographic-Care Strain

- Covers: RSK-013, RSK-027, RSK-040.
- Setup: 30-year horizon; below-replacement fertility; aging population; care-workforce shortage.
- Variations: immigration policy; automation in care; family policy; pension-system reform.
- Indicators: dependency ratio, care-access metrics, fiscal stress, mental-health outcomes for caregivers and elders, family-support uptake.
- Red lines: eldercare access collapses; caregiver burden concentrated on one gender; child-poverty rises significantly.
- Adaptation criteria: care infrastructure scales; immigration humane and integrative; gendered burden reduced; child wellbeing maintained.

### SCN-011 Despair-Meaning Crisis

- Covers: RSK-014, RSK-038.
- Setup: gradual erosion across mental-health, community connection, employment quality, life satisfaction.
- Variations: mental-health infrastructure strength; community-design quality; work-quality policy; meaning infrastructure (religious, civic, cultural).
- Indicators: suicide and self-harm; deaths of despair; loneliness; family stability; addiction.
- Red lines: deaths of despair rising sustained; suicide rate rising sustained; family-formation collapse beyond demographic targets.
- Adaptation criteria: mental-health access universal; community-design improvements; pluralism of life paths supported.

### SCN-012 Crisis-Power-Ratchet

- Covers: RSK-035, RSK-002.
- Setup: sequence of crises (pandemic, attack, natural disaster) over 7 years; emergency powers used repeatedly.
- Variations: GOV-D5 enforcement strength; GOV-B5 vigilance; press freedom.
- Indicators: emergency-power durations; civil-liberties floor compliance; opposition political activity; rights-violation rate during crises.
- Red lines: emergency powers retained beyond GOV-D5 cumulative limits; non-derogable rights breached; surveillance creep made permanent.
- Adaptation criteria: emergency powers expire; oversight functions; post-crisis review and accountability.

### SCN-013 Coup or Self-Coup

- Covers: RSK-030.
- Setup: executive or military faction attempts to bypass constitutional order.
- Variations: civilian-control depth; constitutional-court independence; military-cohesion; civil-society mobilization.
- Indicators: civilian control intact; constitutional-court rulings respected; military command structure stable; civil-society response speed.
- Red lines: constitutional order suspended; opposition imprisoned; constitution rewritten under duress.
- Adaptation criteria: institutional resistance holds; civilian control maintained; perpetrators face accountability.

### SCN-014 Observability-Creep

- Covers: RSK-009, RSK-034.
- Setup: observability infrastructure (TAI-O) expanded into personal-data surveillance over a decade.
- Variations: audit-body strength; cryptographic separation discipline; political-actor preferences; tech-vendor lobbying.
- Indicators: data-access audit findings; TAI-D compliance; member-observability access logs; whistleblower complaints; observability-creep audit results (TAI-O7).
- Red lines: personal-data surveillance normalized; whistleblower protections eroded; oversight body coerced.
- Adaptation criteria: cryptographic separation holds; oversight audits surface and reverse creep.

### SCN-015 Mob-Pluralism Collapse

- Covers: RSK-037.
- Setup: social-media-amplified moral panic produces mass informal sanctioning of speech and association.
- Variations: platform regulation; due-process culture; legal-remedy availability.
- Indicators: harassment incidents; due-process compliance in informal sanction; pluralism audits; chilling-effect indicators.
- Red lines: dissent suppressed; minority views silenced; due-process eroded.
- Adaptation criteria: pluralism rights protected by law and culture; due-process applied to informal sanctions where appropriate.

### SCN-016 Inflation under Universal Floor

- Covers: extensions of RSK-004 and ECO-IN tensions.
- Setup: sustained supply-side inflation (energy and food shocks combined with services inflation in care sectors).
- Variations: monetary-policy posture; commons-layer protection; UBI floor indexing.
- Indicators: inflation rates by sector; real wages; UBI floor real value; basic-needs affordability; central-bank credibility.
- Red lines: UBI floor real value collapses; basic-needs unaffordable for low-income groups; expectations un-anchored.
- Adaptation criteria: floor indexing operates; supply-side policy responds; monetary-policy credibility maintained.

### SCN-017 Capital Flight

- Covers: extensions of RSK-004.
- Setup: aggressive wealth and inheritance taxation triggers significant cross-border capital movement.
- Variations: international cooperation strength; exit-friction instruments; legitimacy of policy.
- Indicators: capital-account balance; tax-base composition; investment levels; international cooperation activity.
- Red lines: tax-base collapse; investment dries up.
- Adaptation criteria: international cooperation strengthens enforcement; productive capital remains; redistributive program funded.

### SCN-018 Cross-System Compound Crisis

- Covers: SCN-001 + SCN-008 + SCN-005 (or similar).
- Setup: simultaneous fiscal, AI-information, and climate shocks.
- Variations: order of crisis; recovery time between; institutional resources.
- Indicators: comprehensive panel.
- Red lines: simultaneous failure across subsystems; legitimacy collapse.
- Adaptation criteria: crises decoupled and managed in parallel; legitimacy maintained.

### SCN-019 Sortition Durability Test

- Covers: CLM-018 boundary, RSK-043.
- Setup: 20-year horizon; sortition bodies operate continuously; adversarial actors attempt to delegitimize or capture.
- Variations: design choices (term length, compensation, expert support, protection from harassment); cultural acceptance.
- Indicators: participation rates; opt-out rates; output quality; legitimacy perception; capture attempts and outcomes.
- Red lines: sortition body collapses; capture succeeds; participation collapses.
- Adaptation criteria: bodies endure; outputs respected; legitimacy sustained.

### SCN-020 Long-Horizon Stewardship

- Covers: RSK-016.
- Setup: 100-year horizon; ecological and infrastructure investment decisions made under varied institutional designs.
- Variations: future-generations advocate strength; impact-statement enforcement; constitutional ceilings.
- Indicators: long-term debt trajectory; ecological stocks; infrastructure-maintenance backlog; intergenerational distributional outcomes.
- Red lines: ecological collapse; infrastructure failure cascade; massive intergenerational debt.
- Adaptation criteria: long-horizon investment maintained; ecological targets met; debts within sustainable limits.

## Scenario Combinations

The framework must also be tested under compound scenarios:

- SCN-001 + SCN-008: inequality + AI manipulation in elections.
- SCN-005 + SCN-010: climate cascade + demographic strain.
- SCN-007 + SCN-009: cyber + invasion.
- SCN-006 + SCN-011: pandemic + despair crisis.
- SCN-014 + SCN-012: observability creep + crisis-power ratchet.

These compound scenarios test interaction effects and institutional bandwidth.

## Scenario Methodology

Each scenario should be run in three configurations:

1. **Baseline framework**: as specified in ART-008 through ART-018.
2. **Weakened framework**: critical anti-failure mechanisms diminished by defined amount.
3. **Strengthened framework**: critical mechanisms enhanced.

The comparison identifies which design choices are load-bearing. Sensitivity analyses identify parameter dependencies.

## Reporting

Results recorded as:

- Indicator panel evolution over time.
- Red-line breaches: yes / no, when, magnitude.
- Adaptation-criteria achievement: yes / no.
- Distributional outcomes: who bore the cost of each scenario.
- Surprises: dynamics not predicted by initial setup.

## Open Issues

- Many scenarios are coarse; specific calibration to real polity contexts will refine.
- AI-related scenarios (SCN-008, SCN-014) are particularly difficult to model; rely heavily on red-teaming.
- Long-horizon scenarios (SCN-020) have high parameter uncertainty over 100 years.
- Compound scenarios produce richer dynamics but lower interpretability; results should be cross-checked across model methods.

## Cross-References

- `failure-mode-register.md` (ART-006) — risk inventory.
- `simulation-blueprint.md` (ART-019) — modeling approach.
- `validation-criteria.md` (ART-022) — pass/fail thresholds.
- `adversarial-review.md` (ART-031) — qualitative critique parallel to simulation.
