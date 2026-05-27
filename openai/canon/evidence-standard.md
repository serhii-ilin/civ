# Evidence Standard

## Claim Classification

Every empirical or causal claim must be tagged as one of:

- `[ESTABLISHED]`: supported by multiple credible sources, replications, long-running data, or broad expert consensus.
- `[CONTESTED]`: supported by some evidence but materially disputed by credible sources.
- `[THEORETICAL]`: plausible based on formal reasoning, models, or extrapolation but not directly validated.
- `[ASSUMPTION]`: necessary premise that is not yet established.
- `[NORMATIVE]`: value judgment that cannot be settled empirically.

## Source Requirements

Use citations for every empirical claim. Prefer:

- Peer-reviewed meta-analyses and systematic reviews.
- Government, intergovernmental, or statistical agency datasets.
- Historical primary sources or reputable academic histories.
- Replication studies, longitudinal data, and natural experiments.
- Transparent models with inspectable assumptions.

Avoid relying on:

- Single unsourced essays for empirical claims.
- Advocacy material without independent corroboration.
- Anecdotes unless clearly labeled as illustrative.
- Claims that cannot be traced to a source or model.

## Evidence Table Format

Each major artifact should include or reference an evidence table:

| Claim ID | Claim | Classification | Source(s) | Confidence | Notes |
| --- | --- | --- | --- | --- | --- |
| CLM-001 | Example claim | [ESTABLISHED] | Source list | High | Boundary conditions |

## Assumption Register

All assumptions must be recorded:

| Assumption ID | Statement | Used In | Test Method | Failure Signal | Status |
| --- | --- | --- | --- | --- | --- |
| ASM-001 | Example assumption | GOV-001 | Simulation or historical comparison | Metric threshold crossed | Open |

## Contradiction Handling

When an internal contradiction appears:

1. Assign a contradiction ID.
2. Name the affected modules and values.
3. Explain the contradiction without resolving it prematurely.
4. Propose resolution options.
5. Identify evidence, stakeholder input, or simulation needed.
6. Record the final decision only after rationale is explicit.

## Decision Log Format

| Decision ID | Date | Scope | Decision | Alternatives | Rationale | Evidence | Revisit Trigger |
| --- | --- | --- | --- | --- | --- | --- | --- |
| DEC-001 | YYYY-MM-DD | GOV-001 | Example decision | Options considered | Why chosen | Source or model | Trigger |
