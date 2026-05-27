# Artifact Structure

Artifacts are the concrete outputs of each research iteration. They live under:

```text
iterations/<iteration_id>/artifacts/
```

All artifact paths are relative to the current agent folder. Do not prefix artifact paths with any provider or agent folder name.

Each iteration must include an artifact manifest that records artifact IDs, paths, status, change type, dependencies, and whether the artifact is required for the active run mode.

## Required Artifact Tree

```text
artifacts/
  00-executive-summary.md
  01-framework-manifesto.md
  research/
    source-register.md
    evidence-matrix.md
    benchmark-catalog.md
    failure-mode-register.md
    behavioral-foundations.md
  architecture/
    value-constitution.md
    governance-system.md
    economic-system.md
    law-and-justice-system.md
    health-and-mental-health-system.md
    education-system.md
    community-and-culture-system.md
    ecology-and-infrastructure-system.md
    technology-and-ai-governance.md
    defense-and-external-relations.md
    technical-architecture.md
  simulation/
    simulation-blueprint.md
    model-parameters.yaml
    stress-test-scenarios.md
    validation-criteria.md
    validation-report.md
  implementation/
    implementation-roadmap.md
    adoption-playbook.md
    governance-migration-plan.md
  review/
    decision-log.md
    assumption-register.md
    contradiction-register.md
    risk-register.md
    adversarial-review.md
    change-log.md
```

## Artifact Contracts

### ART-001 Executive Summary

Path: `00-executive-summary.md`

Required sections:

- Purpose.
- What changed in this iteration.
- Highest-confidence findings.
- Most important unresolved questions.
- Major risks and contradictions.
- Recommended next iteration.

### ART-002 Framework Manifesto

Path: `01-framework-manifesto.md`

Human-readable 5-10 page synthesis of values, goals, institutions, and societal design.

### ART-018 Technical Architecture

Path: `architecture/technical-architecture.md`

Detailed specification of governance, economy, law, health, education, community, ecology, technology, defense, and simulation interfaces.

### ART-008 Value Constitution

Path: `architecture/value-constitution.md`

Formal values, definitions, indicators, conflict-resolution rules, amendment rules, and value tradeoffs.

### ART-003 Source Register

Path: `research/source-register.md`

| Source ID | Citation | URL/DOI | Type | Used In | Reliability Notes |
| --- | --- | --- | --- | --- | --- |
| SRC-001 | Example | Example | Meta-analysis | CLM-001 | Notes |

### ART-004 Evidence Matrix

Path: `research/evidence-matrix.md`

| Claim ID | Claim | Classification | Source IDs | Confidence | Used In |
| --- | --- | --- | --- | --- | --- |
| CLM-001 | Example claim | [ESTABLISHED] | SRC-001 | High | GOV-001 |

### ART-006 Failure Mode Register

Path: `research/failure-mode-register.md`

| Risk ID | Failure Mode | Historical Examples | Mechanism | Mitigations | Residual Risk | Test |
| --- | --- | --- | --- | --- | --- | --- |
| RSK-001 | Elite capture | Examples | Mechanism | Mitigation | Residual | Stress test |

### ART-019 Simulation Blueprint

Path: `simulation/simulation-blueprint.md`

Required sections:

- Model type and rationale.
- Agent types.
- Behavioral rules.
- Institutional rules.
- Resource flows.
- Metrics.
- Stress scenarios.
- Validation thresholds.
- Known model limitations.

### ART-024 Implementation Roadmap

Path: `implementation/implementation-roadmap.md`

Required sections:

- Minimum viable pilot.
- 1-year, 5-year, and 20-year adoption paths.
- Legal dependencies.
- Economic dependencies.
- Governance dependencies.
- Community onboarding.
- Exit and rollback mechanisms.

### ART-027 Decision Log

Path: `review/decision-log.md`

| Decision ID | Scope | Decision | Alternatives | Rationale | Evidence | Revisit Trigger |
| --- | --- | --- | --- | --- | --- | --- |
| DEC-001 | GOV-001 | Example | Options | Rationale | CLM-001 | Trigger |

### ART-028 Assumption Register

Path: `review/assumption-register.md`

| Assumption ID | Statement | Used In | Test Method | Failure Signal | Status |
| --- | --- | --- | --- | --- | --- |
| ASM-001 | Example | ECO-001 | Simulation | Threshold crossed | Open |

### ART-031 Adversarial Review

Path: `review/adversarial-review.md`

Required review perspectives:

- Skeptic.
- Historian.
- Behavioral scientist.
- Institutional-abuse reviewer.
- Civil-liberties reviewer.
- Ecological-systems reviewer.

## Status Values

Artifact status must be one of:

- `pending`
- `draft`
- `reviewed`
- `validated`
- `superseded`
- `deprecated`

Artifact change type must be one of:

- `new`
- `changed`
- `unchanged`
- `superseded`
- `deprecated`

## Change Policy

For targeted iterations, produce only changed artifacts plus required review artifacts. The artifact manifest must list unchanged dependencies so a reader can reconstruct the full framework state.
