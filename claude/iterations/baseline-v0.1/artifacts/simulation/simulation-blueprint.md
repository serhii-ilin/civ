# Simulation Blueprint

Artifact ID: ART-019
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: MOD-SIM
Depends on: ART-018

## Purpose

Specify how the civilization framework can be stress-tested through computational modeling and qualitative analysis. The blueprint defines the model type, agent types, behavioral rules, institutional rules, resource flows, metrics, stress scenarios, validation thresholds, and known model limitations.

This artifact is a design specification, not an implementation. Implementations may use different ABM frameworks (Mesa, NetLogo, Repast, custom) and different system-dynamics tools depending on the question.

## Model Type and Rationale

### SIM-T1 Hybrid Multi-Method Approach

The framework cannot be validated by any single model class. The blueprint adopts a hybrid:

- **Agent-based models (ABM)** for: distributional dynamics, network effects, emergent inequality, trust evolution, polarization, segregation, cooperation under varied institutional rules, electoral dynamics.
- **System dynamics (SD) / integrated assessment** for: aggregate flows of money, energy, materials, emissions, demography, ecological stocks.
- **Network models** for: cyber-resilience, supply chains, social networks, influence cascades, contagion (disease, panic, information).
- **Game-theoretic and mechanism-design analysis** for: voting rules, antitrust dynamics, tax response, deterrence equilibria, sortition incentive compatibility.
- **Qualitative scenario analysis and red-teaming** for: AI risks, adversarial actor strategies, cultural change, long-horizon institutional decay.
- **Historical comparison** for: validating model behavior against documented past episodes (BMK-001 to BMK-013).

Rationale: complex social systems exceed any one method's modeling capacity (CLM-153). Hybrid methods cross-validate and identify model-specific artifacts.

### SIM-T2 Modelable vs. Non-Modelable

Several framework elements cannot be reliably modeled and must be tested by other means:

- AI risks at frontier capability (RSK-010): scenario analysis and red-teaming only.
- Cultural and norm change at societal scale (RSK-014, RSK-017, RSK-038): qualitative and historical analysis.
- Deep moral and legitimacy questions (TZ-007 future generations, TZ-002 anti-pluralism, customary law): deliberative review.
- Specific judicial decisions and rights interpretations: case-by-case analysis.

The framework explicitly admits these limits (CLM-189 plus general epistemic humility).

## Agent Types (SIM-A)

Agent-based models in this framework use a typed agent population. Specific runs may use subsets.

### SIM-A1 Members

- Attributes: age, household, education, occupation, income, wealth, location (cell), health status, mental-health status, trust dimensions, value-orientation, network ties, civic participation history.
- Behavior: bounded-rational; conditional cooperation (B-003); status-and-fairness sensitive (B-002); time-discount with malleability under institutional supports (B-011); occasional deviation from typical patterns.

### SIM-A2 Households

- Composition: one or more members with shared budget and care relationships.
- Decisions: housing, education, savings, consumption, family formation.

### SIM-A3 Firms

- Types: private for-profit (small, medium, large), cooperative, social enterprise, public enterprise.
- Decisions: hiring, pricing, investment, market entry/exit, compliance, lobbying.

### SIM-A4 Government Bodies

- Tiers: local, regional, national.
- Decisions: legislation, regulation, budget, enforcement, services delivery.

### SIM-A5 Non-Profit and Civic Organizations

- Types: associations, religious groups, advocacy, professional bodies, unions, cooperatives.
- Decisions: membership recruitment, participation, advocacy, services.

### SIM-A6 External Actors

- Foreign states, multinational corporations, migrants, refugees, climate-driven shocks.

### SIM-A7 Infrastructure and Ecological Stocks

- Energy systems, water systems, food systems, transport, communications, ecological stocks (forest, fishery, soil, biodiversity).

## Behavioral Rules (SIM-B)

### SIM-B1 Decision Heuristics

- Members use bounded-rationality heuristics: satisficing, similarity-based, social-conformity-weighted, recency-biased.
- Mix of strategies in population; no one heuristic dominates.

### SIM-B2 Cooperation

- Conditional cooperation: members cooperate when observed cooperation rate around them exceeds threshold; defect when below.
- Punishment cost for observed defection partially internalized (B-006); enforcement effectiveness depends on institutional design.

### SIM-B3 Status and Procedural Fairness

- Behavior weighted by perceived procedural fairness (Tyler, CLM-090): compliance, voice, trust increase with perceived fairness; protest, withdrawal, evasion increase with perceived unfairness.

### SIM-B4 Information Flow

- Members update beliefs from local observation (network neighbors), institutional reports, and media (which itself is modeled).
- Information environment modeled with content-quality and source-trust attributes.

### SIM-B5 Voting and Civic Participation

- Voting and participation rates vary by demographic, locality, perceived efficacy.
- Sortition selection randomizes from member population subject to opt-out fraction.

### SIM-B6 Migration

- Members migrate within polity (between cells) based on opportunity differentials.
- External migration modeled as shock and ongoing flow.

### SIM-B7 Care, Family, Reproduction

- Caregiving allocation modeled with policy-dependent burden distribution.
- Family formation and reproduction modeled with policy-dependent rates.

### SIM-B8 Health Behaviors

- Health behaviors influenced by environment, education, network, access to services.

### SIM-B9 Defection from Institutions

- Members can withdraw consent (refuse to participate, leave, organize opposition) when institutional legitimacy falls below threshold.

## Institutional Rules (SIM-I)

### SIM-I1 Governance

- Multi-tier authority per ART-009.
- Decision rules per GOV-D.
- Body composition per GOV-S.
- Capture-resistance mechanisms per GOV-A.

### SIM-I2 Legal Enforcement

- Crime detection and adjudication rates per LAW.
- Sanctions per LAW-CJ.
- Civil-dispute resolution per LAW-CV / CUL-CR.

### SIM-I3 Economic

- Tax instruments per ECO-T.
- Commons and public-provisioning layers per ECO-L.
- Antitrust enforcement per ECO-MK1.

### SIM-I4 Ecological

- Hard caps per ECN-B.
- Allocation mechanisms per ECN-B3.
- Land-tenure rules per ECN-L.

### SIM-I5 Health

- Universal access per HEA-A1.
- Pandemic response per HEA-P3.

### SIM-I6 Education

- Pathways and equity per EDU-P, EDU-E.

### SIM-I7 Technology / AI

- Risk-tier enforcement per TAI-R.
- Data rights per TAI-D.

### SIM-I8 Defense

- Threat response per DEF.
- Crisis powers per DEF-C.

## Resource and Material Flows (SIM-R)

### SIM-R1 Energy

- Generation by type; transmission; consumption by sector.
- Constraints per ECN-E.

### SIM-R2 Water

- Withdrawal, treatment, distribution, return; watershed accounts.
- Constraints per ECN-W.

### SIM-R3 Food

- Production, distribution, consumption; nutrient and caloric balance.
- Constraints per ECN-F.

### SIM-R4 Materials

- Material throughput; circular vs. linear flows.
- Constraints per ECN-M.

### SIM-R5 Financial

- Money, credit, savings, investment flows.
- Banking constraints per ECO-M.

### SIM-R6 Demographic

- Births, deaths, migration; age-structure evolution.

### SIM-R7 Ecological Stocks

- Soil, forests, fisheries, biodiversity, climate.

## Metrics (SIM-M)

### SIM-M1 Core Indicator Panel

Aligned with `value-constitution.md` indicators and `technical-architecture.md` (TAR-Q):

- Inequality: Gini, top-decile share, wealth concentration.
- Wellbeing: subjective wellbeing, capability index, time-poverty.
- Health: life expectancy, healthy life years, preventable burden, mental health treatment access, loneliness.
- Education: literacy, capability assessments, mobility.
- Governance: trust in institutions, perceived procedural fairness, recall and removal rates.
- Rights: rights-violation rate, due-process completion.
- Ecology: emissions, material footprint, biodiversity, water stress.
- Resilience: reserve durations, recovery times, supply-chain concentration.
- Innovation: research intensity, new-firm rates, productivity.
- Care: caregiver-burden distribution, child wellbeing, elder isolation.
- Pluralism: discrimination rate, exit/voice rates, minority-rights audit.
- Observability: decision-log completeness, audit-response rate, observability-creep audit results.
- External: foreign-influence detected, alliance and trade metrics, migration outcomes.

### SIM-M2 Distributional Reporting

- All indicators reported with distribution, not only mean.
- Quantile disparities tracked.
- Sub-group disparities (region, demographic) tracked.

### SIM-M3 Time Horizon

- Short-run: 1-3 years.
- Medium-run: 4-10 years.
- Long-run: 11-50 years.
- Multi-generational: 50-200 years for ecological and intergenerational stewardship.

### SIM-M4 Goodhart-Aware Reporting

- No indicator is the sole driver of a simulated decision (CLM-189).
- Indicators are audited for gaming; perverse-incentive analysis runs alongside.

## Stress Scenarios

Detailed in `stress-test-scenarios.md` (ART-021). Each scenario references one or more failure modes from `failure-mode-register.md`.

## Validation Thresholds

Detailed in `validation-criteria.md` (ART-022). The framework is considered:

- Robust if indicator-panel results survive most stress scenarios within defined bounds.
- Vulnerable if indicator-panel results breach red lines in defined scenarios.

## Model Limitations (SIM-LIM)

### SIM-LIM1 Behavioral Simplification

- Real human behavior is richer than any decision rule; models are caricatures.
- Cross-cultural variation under-represented (CLM-060).

### SIM-LIM2 Emergent Phenomena

- Some emergent dynamics (cultural change, norm shifts) operate on timescales and through mechanisms not well captured in ABM.

### SIM-LIM3 Adversaries

- Sophisticated adversaries (state, criminal, AI-enabled) outpace model design; supplement with red-teaming.

### SIM-LIM4 Parameter Uncertainty

- Many parameters are uncertain by 50% or more; sensitivity analysis required (`validation-criteria.md`).

### SIM-LIM5 Path Dependence

- Initial conditions and history matter; the model cannot tell us about polities with very different starting conditions without retuning.

### SIM-LIM6 False Precision

- Results are directional, not point predictions.
- Report ranges, not point estimates, in framework-level conclusions.

### SIM-LIM7 Ethics of Simulation

- Simulating populations raises ethical considerations even with synthetic agents.
- Real-population data used in calibration must respect TAI-D protections.
- Public-good models must be themselves transparent.

## Implementation Notes (SIM-IMP)

### SIM-IMP1 Software

- Recommended ABM: Mesa (Python) for ease of community contribution; NetLogo for prototyping; Repast for high-performance large-scale.
- System dynamics: open tools (Vensim alternatives, SDeverywhere, BPTK) preferred for replicability.
- Network: NetworkX, igraph.
- Game theory: any sufficient library.

### SIM-IMP2 Reproducibility

- All code open-source.
- Parameter files versioned (see `model-parameters.yaml`, ART-020).
- Seeds recorded.
- Multi-run reporting (no single-run conclusions).

### SIM-IMP3 Modularity

- Modules per subsystem; can be combined in different runs.
- Standard interfaces between modules.

### SIM-IMP4 Calibration

- Calibrated against historical data where available.
- Stylized facts (Gini ranges, mobility coefficients, mortality rates, etc.) as anchors.
- Failure to reproduce known stylized facts is a model-disqualifying condition.

### SIM-IMP5 External Review

- Models published with documentation and parameters.
- External review by adversarial-review body (GOV-B5 analogue in implementation).

## Open Issues

- The blueprint specifies many model types but does not commit to specific implementations; that is intentional. Future iterations should specify which models exist, where, and at what maturity.
- Calibration data for many indicators is sparse; this limits validation strength in the baseline.
- The relationship between simulation results and actual policy decisions must be carefully managed (false precision risk).

## Cross-References

- `model-parameters.yaml` (ART-020) — concrete parameters.
- `stress-test-scenarios.md` (ART-021) — concrete scenarios.
- `validation-criteria.md` (ART-022) — thresholds and red lines.
- `validation-report.md` (ART-023) — placeholder report at this iteration.
