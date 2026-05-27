# Artifact Manifest

Iteration: `baseline-v0.1`

Artifact root: `artifacts/`

## Status Legend

- `pending`: not generated yet.
- `draft`: generated but not reviewed.
- `reviewed`: reviewed for evidence, consistency, and contradictions.
- `validated`: supported by simulation, external review, or explicit acceptance criteria.
- `superseded`: replaced by a newer artifact.
- `deprecated`: no longer part of the active framework.

## Required Artifacts

| Artifact ID | Path | Status | Change Type | Owner Module | Dependencies | Required for Run Mode |
| --- | --- | --- | --- | --- | --- | --- |
| ART-001 | artifacts/00-executive-summary.md | draft | new | all | all | yes |
| ART-002 | artifacts/01-framework-manifesto.md | draft | new | all | ART-008, ART-018 | yes |
| ART-003 | artifacts/research/source-register.md | draft | new | MOD-RES | none | yes |
| ART-004 | artifacts/research/evidence-matrix.md | draft | new | MOD-RES | ART-003 | yes |
| ART-005 | artifacts/research/benchmark-catalog.md | draft | new | MOD-RES | ART-003, ART-004 | yes |
| ART-006 | artifacts/research/failure-mode-register.md | draft | new | MOD-RES | ART-003, ART-004 | yes |
| ART-007 | artifacts/research/behavioral-foundations.md | draft | new | MOD-RES | ART-003, ART-004 | yes |
| ART-008 | artifacts/architecture/value-constitution.md | draft | new | all | canon/values.md | yes |
| ART-009 | artifacts/architecture/governance-system.md | draft | new | MOD-GOV | ART-008 | yes |
| ART-010 | artifacts/architecture/economic-system.md | draft | new | MOD-ECO | ART-008 | yes |
| ART-011 | artifacts/architecture/law-and-justice-system.md | draft | new | MOD-LAW | ART-008, ART-009 | yes |
| ART-012 | artifacts/architecture/health-and-mental-health-system.md | draft | new | MOD-HMH | ART-008 | yes |
| ART-013 | artifacts/architecture/education-system.md | draft | new | MOD-EDU | ART-008, ART-012 | yes |
| ART-014 | artifacts/architecture/community-and-culture-system.md | draft | new | MOD-CUL | ART-008, ART-011, ART-012 | yes |
| ART-015 | artifacts/architecture/ecology-and-infrastructure-system.md | draft | new | MOD-ECOINF | ART-008, ART-010 | yes |
| ART-016 | artifacts/architecture/technology-and-ai-governance.md | draft | new | MOD-TAI | ART-008, ART-009, ART-011 | yes |
| ART-017 | artifacts/architecture/defense-and-external-relations.md | draft | new | MOD-DEF | ART-008, ART-009, ART-011 | yes |
| ART-018 | artifacts/architecture/technical-architecture.md | draft | new | all architecture modules | ART-008 through ART-017 | yes |
| ART-019 | artifacts/simulation/simulation-blueprint.md | draft | new | MOD-SIM | ART-018 | yes |
| ART-020 | artifacts/simulation/model-parameters.yaml | draft | new | MOD-SIM | ART-009 through ART-017 | yes |
| ART-021 | artifacts/simulation/stress-test-scenarios.md | draft | new | MOD-SIM | ART-006, ART-018 | yes |
| ART-022 | artifacts/simulation/validation-criteria.md | draft | new | MOD-SIM | ART-019, ART-020, ART-021 | yes |
| ART-023 | artifacts/simulation/validation-report.md | draft | new | MOD-SIM | ART-019, ART-020, ART-021, ART-022 | yes |
| ART-024 | artifacts/implementation/implementation-roadmap.md | draft | new | all architecture modules | ART-018 | yes |
| ART-025 | artifacts/implementation/adoption-playbook.md | draft | new | all architecture modules | ART-024 | yes |
| ART-026 | artifacts/implementation/governance-migration-plan.md | draft | new | MOD-GOV, MOD-LAW | ART-009, ART-011, ART-024 | yes |
| ART-027 | artifacts/review/decision-log.md | draft | new | all | none | yes |
| ART-028 | artifacts/review/assumption-register.md | draft | new | all | none | yes |
| ART-029 | artifacts/review/contradiction-register.md | draft | new | all | none | yes |
| ART-030 | artifacts/review/risk-register.md | draft | new | all | ART-006 | yes |
| ART-031 | artifacts/review/adversarial-review.md | draft | new | all | ART-018 | yes |
| ART-032 | artifacts/review/change-log.md | draft | new | all | none | yes |

## Manifest Rules

Every generated artifact must be listed here. Targeted iterations may list unchanged dependencies as `reviewed` or `validated` without regenerating them.
