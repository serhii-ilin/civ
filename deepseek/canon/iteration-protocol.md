# Iteration Protocol

## Stable IDs

Use stable IDs for all reusable components:

- Values: `VAL-001`
- Modules: `MOD-GOV`, `MOD-ECO`, `MOD-SIM`
- Research questions: `RQ-GOV-001`
- Claims: `CLM-001`
- Sources: `SRC-001`
- Assumptions: `ASM-001`
- Decisions: `DEC-001`
- Risks: `RSK-001`
- Contradictions: `CON-001`
- Artifacts: `ART-001`

## Run Modes

### full_research

Use when creating a new baseline or when the whole framework must be regenerated.

Required outputs:

- All artifact groups in `artifact-structure.md`.
- Updated source register.
- Updated decision log.
- Updated assumption register.
- Phase-level adversarial review.

### module_update

Use when revising one or more modules.

Required outputs:

- Changed artifacts only.
- Diff summary against `compare_against`.
- Updated decisions, assumptions, contradictions, and risks for the selected modules.
- Compatibility check against locked sections.

### adversarial_review

Use when testing an existing iteration without rewriting it.

Required outputs:

- Findings ordered by severity.
- Affected artifact IDs.
- Evidence gaps.
- Proposed fixes.
- Residual risk.

### simulation_update

Use when changing validation methods, parameters, scenarios, or thresholds.

Required outputs:

- Updated simulation blueprint.
- Parameter changes.
- Scenario changes.
- Validation criteria changes.
- Impacts on assumptions and decisions.

### implementation_update

Use when changing adoption strategy, roadmap, institutional migration, or operational procedures.

Required outputs:

- Updated implementation roadmap.
- Adoption risks.
- Dependency changes.
- Governance or legal compatibility notes.

## Run Configuration

Each iteration must define:

```yaml
iteration_id: baseline-v0.1
run_mode: full_research
compare_against: null
focus_modules:
  - MOD-RES
  - MOD-GOV
  - MOD-ECO
  - MOD-LAW
  - MOD-HMH
  - MOD-EDU
  - MOD-CUL
  - MOD-ECOINF
  - MOD-TAI
  - MOD-DEF
  - MOD-SIM
locked_sections:
  - canon/mission.md
  - canon/values.md
  - canon/evidence-standard.md
output_policy:
  changed_sections_only: false
  include_decision_log: true
  include_assumption_register: true
  include_source_register: true
  include_adversarial_review: true
```

## Completion Criteria

An iteration is complete only when:

- All selected modules have produced their required artifacts.
- Every empirical claim is classified and sourced.
- All assumptions are registered.
- All major design choices are recorded in the decision log.
- Contradictions are either resolved with rationale or preserved as open issues.
- The artifact manifest lists every produced file and its status.
