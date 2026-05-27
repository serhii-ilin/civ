# Simulation Blueprint

Iteration: `baseline-v0.1`

Status: `draft`

Artifact: `ART-019`

## Model Type and Rationale

Use a hybrid model:

- Agent-based model for households, communities, institutions, firms, officials, and external actors.
- System-dynamics layer for stocks and flows: food, water, energy, fiscal capacity, ecological load, trust, health capacity, and infrastructure condition.
- Scenario engine for shocks and policy changes.
- Qualitative review layer for rights, legitimacy, legal doctrine, and moral tradeoffs that should not be reduced to a score.

This combination avoids false precision while allowing stress tests of feedback loops and failure modes.

## Agent Types

| Agent ID | Agent | Key State Variables |
| --- | --- | --- |
| AG-001 | Household | Income, health, skills, trust, social ties, care burden, preparedness, location. |
| AG-002 | Community cell | Service capacity, cohesion, conflict load, reserves, leadership quality, observability score. |
| AG-003 | Public institution | Budget, competence, legitimacy, corruption exposure, backlog, audit status. |
| AG-004 | Firm or cooperative | Employment, productivity, market share, ecological footprint, ownership form. |
| AG-005 | Review body | Detection capacity, independence, backlog, enforcement success. |
| AG-006 | External actor | Trade reliability, hostility, cyber capability, migration pressure, alliance status. |

## Behavioral Rules

- Cooperation depends on trust, legitimacy, enforcement fairness, local ties, and perceived reciprocity.
- Institutional performance affects trust with lag and asymmetric loss from abuse or failure.
- Wealth and influence can compound into capture unless constrained.
- Health, stress, education, and childhood conditions affect capability and participation.
- Ecological overshoot raises infrastructure, food, health, and conflict risks.

## Institutional Rules

- Rights-floor violations trigger legal review and legitimacy loss.
- Emergency powers expire unless renewed and reviewed.
- Audit bodies detect capture probabilistically based on independence, observability, and workload.
- Ecological caps constrain production and infrastructure expansion.
- Commons service degradation lowers trust and raises market pressure.

## Resource Flows

Food, water, energy, money, care labor, skills, information, legitimacy, ecological capacity, and security attention are tracked as partially substitutable but not reducible to one welfare score.

## Metrics

- Gini coefficient, wealth concentration, poverty, survival-floor access.
- Trust, participation, appeal outcomes, institutional backlog.
- Rights violations, surveillance incidents, due-process delays.
- Mental-health wait time, loneliness, preventable mortality.
- Carbon budget, water stress, biodiversity proxy, material throughput.
- Reserve duration, recovery time, cyber recovery, supply-chain concentration.
- Education and reskilling access.
- Boundary integrity and emergency-power duration.

## Stress Scenarios

The model must support the scenarios defined in `stress-test-scenarios.md`, with first priority on:

- SCN-003: Elite capture through procurement, media ownership, and campaign finance.
- SCN-004: Pandemic with uncertain early evidence.
- SCN-010: Fiscal downturn plus infrastructure decay.

Each scenario must record affected values, invalidated assumptions, redesign triggers, and whether the failure is institutional, resource-based, behavioral, ecological, security-related, or model-design related.

## Validation Thresholds

Initial thresholds are defined in `validation-criteria.md` and parameterized in `model-parameters.yaml`. Thresholds are provisional until calibrated, and any threshold affecting rights or emergency powers requires qualitative legal review in addition to model output.

Minimum validation outputs:

- Pass/fail result for each `VALD-*` criterion.
- Sensitivity analysis for capture, trust, reserve duration, service backlog, ecological caps, and audit detection.
- Identification of assumptions whose failure changes the policy recommendation.
- Explanation of model limits and nonmodeled moral tradeoffs.

## Known Model Limitations

- Moral legitimacy cannot be optimized numerically.
- Historical analogies are not calibration data by themselves.
- Agent rules can hide value assumptions.
- Rare catastrophic events require scenario analysis, not ordinary averages.
- Cultural change and leadership quality are hard to parameterize.
