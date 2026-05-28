# Validation Report

Artifact ID: ART-023
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: MOD-SIM
Depends on: ART-019, ART-020, ART-021, ART-022

## Status

This baseline iteration produces the simulation blueprint, parameters, scenarios, and criteria as artifacts but does not yet contain executed simulation runs. This validation report is therefore a **placeholder** describing the structure and expected content of validation reports produced by future simulation-update iterations.

Future iterations of mode `simulation_update` should populate the sections below with actual run outputs. Each row in the results tables corresponds to one scenario × configuration × run-set combination.

## Run Summary (placeholder)

| Scenario | Config | Runs | Status |
| --- | --- | --- | --- |
| SCN-001 Inequality-Power Feedback | baseline | 0 | not run |
| SCN-001 Inequality-Power Feedback | weakened anti-capture | 0 | not run |
| SCN-001 Inequality-Power Feedback | strengthened anti-capture | 0 | not run |
| SCN-002 Demagogue Ascent | baseline | 0 | not run |
| SCN-002 Demagogue Ascent | captured regulators | 0 | not run |
| SCN-003 Fiscal Shock | baseline | 0 | not run |
| SCN-003 Fiscal Shock | sovereign-wealth available | 0 | not run |
| SCN-004 Cleavage Escalation | baseline | 0 | not run |
| SCN-005 Climate Cascade | baseline | 0 | not run |
| SCN-005 Climate Cascade | depleted reserves | 0 | not run |
| SCN-006 Pandemic | baseline | 0 | not run |
| SCN-007 Cyber Critical-Infrastructure Attack | baseline | 0 | not run |
| SCN-008 AI-Information Shock | baseline | 0 | not run |
| SCN-009 Foreign Invasion | baseline | 0 | not run |
| SCN-010 Demographic-Care Strain | baseline | 0 | not run |
| SCN-011 Despair-Meaning Crisis | baseline | 0 | not run |
| SCN-012 Crisis-Power-Ratchet | baseline | 0 | not run |
| SCN-013 Coup or Self-Coup | baseline | 0 | not run |
| SCN-014 Observability-Creep | baseline | 0 | not run |
| SCN-015 Mob-Pluralism Collapse | baseline | 0 | not run |
| SCN-016 Inflation under Universal Floor | baseline | 0 | not run |
| SCN-017 Capital Flight | baseline | 0 | not run |
| SCN-018 Cross-System Compound Crisis | baseline | 0 | not run |
| SCN-019 Sortition Durability Test | baseline | 0 | not run |
| SCN-020 Long-Horizon Stewardship | baseline | 0 | not run |

## Indicator Panel (placeholder)

For each scenario × configuration, the panel reports:

| Indicator | Year 5 | Year 10 | Year 25 | Year 50 | Red Line? |
| --- | --- | --- | --- | --- | --- |
| Gini (post-tax-transfer) | — | — | — | — | — |
| Top-decile income share | — | — | — | — | — |
| Trust in institutions | — | — | — | — | — |
| Loneliness rate | — | — | — | — | — |
| Healthy life expectancy | — | — | — | — | — |
| Mental-health treatment access (urgent) | — | — | — | — | — |
| Upper-secondary completion | — | — | — | — | — |
| Rights-violation rate | — | — | — | — | — |
| GHG emissions vs. budget | — | — | — | — | — |
| Material footprint | — | — | — | — | — |
| Biodiversity intactness | — | — | — | — | — |
| Reserve durations (food/energy/medicine) | — | — | — | — | — |
| Recovery time after shock | — | — | — | — | — |
| Innovation (new-firm rate) | — | — | — | — | — |
| Care-burden distribution | — | — | — | — | — |
| Discrimination-audit findings | — | — | — | — | — |
| Decision-log completeness | — | — | — | — | — |
| Audit-response rate | — | — | — | — | — |
| Observability-creep audit | — | — | — | — | — |

## Findings Templates

When this report is populated, findings should be reported in the following form:

```text
Finding-ID: FND-001
Scenario: SCN-XXX
Configuration: ...
Result: Pass | Yellow | Red
Red-line breached: yes/no, which one, when
Adaptation criteria: met/missed (list)
Distributional outcomes: who bore the cost
Sensitivity: which parameters move outcome
Surprises: dynamics not predicted
Recommended action: continue / module-update / full-research
```

## Cross-Method Replication (placeholder)

When the framework is simulated, results must be cross-validated across at least two of:

- Agent-based model.
- System dynamics.
- Network model.
- Game-theoretic analysis.
- Qualitative scenario red-teaming.

The report records which methods agree on each finding and where they disagree.

## Historical Comparison (placeholder)

Where applicable, simulation outcomes will be cross-checked against benchmark cases (ART-005). Examples:

- Inequality-feedback dynamics calibrated against Roman Republic (BMK-001) and Gilded Age US.
- Federalism-resilience calibrated against Swiss Confederation (BMK-004).
- Cooperative-scaling calibrated against Mondragon (BMK-020).
- Sortition-durability informed by citizens'-assembly cases (BMK-033).

Disagreement between simulation and historical record requires explanation and may trigger model adjustment.

## Open Issues for Future Simulation Iterations

- Choice of ABM platform and SD platform to be decided in a `simulation_update` iteration.
- Specific calibration data sources (real-polity microdata) to be identified.
- Cross-method replication strategy to be specified.
- Resource availability for long runs (50+ year horizons) to be planned.
- Adversarial red-teaming process to be set up for AI-related scenarios.

## Cross-References

- `simulation-blueprint.md` (ART-019) — modeling approach.
- `model-parameters.yaml` (ART-020) — parameter ranges.
- `stress-test-scenarios.md` (ART-021) — scenarios.
- `validation-criteria.md` (ART-022) — thresholds.
- Future iteration of mode `simulation_update` should populate this report.
