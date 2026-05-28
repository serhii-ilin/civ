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

## Baseline v0.1 Results

The `openai/`, `claude/`, and `deepseek/` workspaces each produced a draft `baseline-v0.1` artifact set under `iterations/baseline-v0.1/artifacts/`. The three runs converge on a common research result: resilient civilization design depends less on a single ideal institution than on anti-capture structure, ecological constraints, care infrastructure, rights enforcement, institutional observability, and explicit correction loops.

None of the baseline runs is validated yet. Each includes simulation scaffolding and stress-test definitions, but executable simulation results and external expert review remain future work.

### Approach Summaries

| Workspace | Research posture | Architecture pattern | Strengths | Main open risks |
| --- | --- | --- | --- | --- |
| `claude/` | Broadest and most enumerated research pass, with 102 sources, 76 evidence-graded claims, 45 failure modes, and 48 scored risks. | High-detail constitutional federation: mixed elections and sortition, eleven national governance bodies, explicit adversarial review, five-layer economy, universal services plus a cash floor, hard ecological ceilings, and extensive observability infrastructure. | Strongest internal traceability, richest failure-mode coverage, and most detailed anti-capture design. | High complexity, reliance on the independence of adversarial review, untested large-scale sortition, uncertain ecological-cap durability, and dependence on international coordination. |
| `deepseek/` | Concrete and implementation-facing, with a strong emphasis on lived community design, cooperative economics, and pilot sequencing. | Human-scale federation built from 100-300 person community cells, regional coordination, national constitutional functions, universal basic services, cooperative and stakeholder enterprise, care infrastructure, and phased voluntary adoption. | Clearest day-to-day social model, strongest cooperative-economy emphasis, and most legible transition narrative. | Transition feasibility remains speculative, behavioral assumptions are demanding, community-cell scale may underfit complex infrastructure, and simulations have not been executed. |
| `openai/` | Leaner and more contradiction-led, emphasizing governance/privacy boundaries, implementation gates, and unresolved assumptions. | Constitutional federation with community, regional, central, and independent-review layers; survival floor, commons infrastructure, regulated markets, strategic reserves, rights-bound AI governance, and pilot-first implementation. | Clearest treatment of observability vs. surveillance, competence gates vs. class hierarchy, and pilot safety checks. | Less granular than the other runs, fiscal design needs deeper modeling, risk coverage is narrower, and privacy/legal architecture needs more detail before a real pilot. |

### Cross-Run Comparison

- `claude/` optimizes for comprehensive architecture and adversarial auditability.
- `deepseek/` optimizes for human-scale community life, cooperative ownership, and practical transition sequencing.
- `openai/` optimizes for correction discipline, privacy boundaries, and pilotable governance controls.
- A strong synthesis would combine Claude's failure-mode breadth, DeepSeek's community/cooperative pilot design, and OpenAI's privacy and implementation discipline.

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

- `openai/`: completed draft `baseline-v0.1` with a concise, contradiction-led architecture and pilot-oriented implementation path.
- `claude/`: completed draft `baseline-v0.1` with the most exhaustive research, architecture, failure-mode, and review coverage.
- `deepseek/`: completed draft `baseline-v0.1` with the strongest community-cell, cooperative-economy, and transition narrative.
- `template/`: reusable workspace skeleton for additional agent runs.

Additional model folders can be added using the same internal structure.
