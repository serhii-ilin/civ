# Civilization Architecture Agent Benchmark

This project explores how different AI agents and models design a better society or civilization when given the same research structure, goals, constraints, and artifact requirements.

The work is both a research exercise and a model-comparison benchmark. Each agent runs independently in its own folder, produces its own civilization architecture, and leaves behind comparable artifacts for review.

## Project Goal

The goal is to design and compare evidence-grounded proposals for a healthier, more resilient, more just, and more observable society.

Each agent is asked to produce a civilization framework that addresses:

- Governance and institutional design.
- Law, justice, rights, legitimacy, and public safety.
- Economic structure, incentives, commons, taxation, and wealth concentration.
- Health, mental health, care, education, and community life.
- Ecology, infrastructure, land use, food, water, energy, and climate resilience.
- Technology, AI governance, data rights, cybersecurity, and observability.
- Defense, diplomacy, migration, external boundaries, and crisis response.
- Simulation, stress testing, validation criteria, and failure modes.

The intent is not to generate utopian fiction. The agents should justify design choices with evidence, historical precedent, behavioral science, falsifiable assumptions, and explicit tradeoff analysis.

## Multi-Agent Structure

Each top-level agent folder is an independent workspace:

```text
.
  openai/
  claude/
  deepseek/
  other-agent/
```

Every agent folder should use the same internal structure:

```text
.
  prd.md
  canon/
  modules/
  iterations/
```

Paths inside each workspace must be relative to that workspace. Artifacts should not include parent folder names. For example, an agent writes to:

```text
iterations/baseline-v0.1/artifacts/
```

not:

```text
openai/iterations/baseline-v0.1/artifacts/
```

This keeps outputs portable and makes comparisons between agents mechanical.

## What Gets Compared

Agent outputs should be compared across:

- Value hierarchy: what the model treats as most important.
- Institutional coherence: whether governance, law, economy, culture, and defense fit together.
- Evidence quality: whether empirical claims are sourced and uncertainty is labeled.
- Failure-mode awareness: whether the design anticipates corruption, capture, collapse, abuse, and unintended consequences.
- Human freedom and dignity: whether the design protects rights, dissent, privacy, exit, and minority groups.
- Observability: whether members can audit government and society-scale processes without creating private-life surveillance.
- Security boundaries: whether the society can protect itself from external physical, cyber, economic, informational, and biosecurity threats.
- Simulation readiness: whether the proposal can be modeled, stress-tested, and revised.
- Implementation realism: whether the design can begin as a pilot or transition path rather than requiring instant civilizational replacement.

## Expected Artifacts

Each agent iteration should produce the artifact tree defined in its own `canon/artifact-structure.md`.

The core outputs include:

- Executive summary.
- Framework manifesto.
- Value constitution.
- Technical architecture.
- Governance system.
- Economic system.
- Law and justice system.
- Health and mental health system.
- Education system.
- Community and culture system.
- Ecology and infrastructure system.
- Technology and AI governance.
- Defense and external relations.
- Simulation blueprint.
- Failure mode register.
- Decision log.
- Assumption register.
- Contradiction register.
- Adversarial review.
- Implementation roadmap.

## Workflow

1. Copy or maintain the same PRD structure in each agent folder.
2. Run each agent from inside its own folder.
3. Generate a baseline iteration, usually `iterations/baseline-v0.1/`.
4. Keep source registers, assumptions, decisions, and contradictions explicit.
5. Compare outputs across agents using the same artifact IDs and review criteria.
6. Run targeted follow-up iterations when one agent exposes a useful idea, contradiction, or failure mode.

## Current Workspaces

- `openai/`: active structured workspace with canon, modules, and baseline iteration config.
- `claude/`: reserved workspace for an independent agent run.

Additional model folders can be added using the same internal structure.
