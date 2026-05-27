# Civilization Architecture Research PRD

This directory defines a reproducible research system for designing and testing a new civilization framework. The PRD is split into stable canon, editable research modules, and versioned iteration artifacts so the same research can be rerun, compared, or partially revised without rewriting the whole prompt.

The structure is intentionally provider-agnostic. Run each agent from inside its own workspace folder. All paths in this spec are relative to that current agent folder and must not include the parent provider folder name.

## Primary Objective

Design a comprehensive, evidence-grounded framework for a resilient human society. The work must integrate empirical research, historical analysis, behavioral science, political theory, economics, ecology, technology governance, law, public health, and systems thinking.

The output is not a utopian fiction exercise. Every design decision must be justified by evidence, historical precedent, formal reasoning, or falsifiable theory. Assumptions must be explicit, versioned, and stress-tested.

## Directory Structure

```text
./
  prd.md
  canon/
    mission.md
    values.md
    evidence-standard.md
    iteration-protocol.md
    artifact-structure.md
  modules/
    research-benchmarking.md
    governance.md
    economy.md
    law-and-justice.md
    health-and-mental-health.md
    education.md
    community-and-culture.md
    ecology-and-infrastructure.md
    technology-and-ai.md
    defense-and-external-relations.md
    simulation.md
  iterations/
    baseline-v0.1/
      run-config.yaml
      research-questions.md
      artifact-manifest.md
      artifacts/
        README.md
```

## Stable Canon

These files should change rarely. They define the durable identity of the research program:

- [Mission](canon/mission.md): role, scope, and operating boundaries.
- [Values](canon/values.md): non-negotiable value constitution draft with stable value IDs.
- [Evidence Standard](canon/evidence-standard.md): citation, evidence grading, assumption labeling, and contradiction handling rules.
- [Iteration Protocol](canon/iteration-protocol.md): how to run full research, module updates, reviews, and simulation updates.
- [Artifact Structure](canon/artifact-structure.md): required output layout, artifact naming, and internal schemas.

## Editable Modules

Each module is independently rerunnable. A new iteration can select one module, several modules, or the full set.

- [Research and Benchmarking](modules/research-benchmarking.md)
- [Governance](modules/governance.md)
- [Economy](modules/economy.md)
- [Law and Justice](modules/law-and-justice.md)
- [Health and Mental Health](modules/health-and-mental-health.md)
- [Education](modules/education.md)
- [Community and Culture](modules/community-and-culture.md)
- [Ecology and Infrastructure](modules/ecology-and-infrastructure.md)
- [Technology and AI](modules/technology-and-ai.md)
- [Defense and External Relations](modules/defense-and-external-relations.md)
- [Simulation](modules/simulation.md)

## Run Modes

Set the active run mode in an iteration's `run-config.yaml`.

```yaml
run_mode: full_research
```

Supported modes:

- `full_research`: rerun all selected research and architecture modules.
- `module_update`: revise only selected modules while respecting locked canon and prior decisions.
- `adversarial_review`: critique existing artifacts without rewriting the whole framework.
- `simulation_update`: update simulation assumptions, scenarios, parameters, and validation criteria.
- `implementation_update`: revise adoption roadmaps and operating procedures.

## Iteration Rules

Every iteration must:

- Declare `iteration_id`, `run_mode`, `focus_modules`, `locked_sections`, and `compare_against`.
- Use stable IDs for values, modules, assumptions, decisions, risks, and artifacts.
- Output only the requested scope unless `run_mode` is `full_research`.
- Preserve unresolved conflicts instead of silently resolving them.
- Update the decision log, assumption register, source register, and change log.
- Distinguish established evidence, contested evidence, theoretical proposals, and assumptions.

## Baseline Iteration

The first iteration is defined in [baseline-v0.1](iterations/baseline-v0.1/run-config.yaml). It runs the full research program and produces the complete artifact set under `iterations/baseline-v0.1/artifacts/`.

Future iterations should copy `baseline-v0.1`, change `iteration_id`, set a narrower `run_mode` when appropriate, and declare which sections are locked.
