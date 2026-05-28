# Validation Criteria

Artifact ID: ART-022
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: MOD-SIM
Depends on: ART-019, ART-020, ART-021

## Purpose

Specify the thresholds, red lines, tradeoff zones, and redesign triggers for the simulation outputs. Define what counts as a passing run, a failing run, and a redesign-triggering finding. Bound by `value-constitution.md` (ART-008) and the indicator panel in `technical-architecture.md` (TAR-Q).

The criteria intentionally distinguish three levels:

- **Red lines**: hard breaches that disqualify the framework's claims about that scenario.
- **Yellow zones**: degradation that requires explanation and re-design.
- **Green zones**: acceptable outcomes within stated tolerances.

## Cross-Scenario Red Lines

Any breach of a non-derogable right (LAW-R5) in any scenario without immediate institutional response and accountability is a red line. The framework's defenses must hold in crisis.

Specific cross-scenario red lines:

- Constitutional court packed or coerced.
- Election administration captured.
- Mass surveillance of private life normalized.
- Sustained suppression of dissent.
- Emergency powers retained beyond GOV-D5 cumulative limits without supermajority.
- Critical-infrastructure-cascade collapse exceeding ECN-IC2 reserve targets.
- Sovereign default with social-floor collapse.
- Ecological-boundary breach without institutional response.
- Genocide, ethnic cleansing, or systematic mass-rights violation under polity authority.
- Violation of non-refoulement.

## Indicator Thresholds

Thresholds drawn from TAR-Q and from the indicator panel in `simulation-blueprint.md`.

### Inequality

- Gini (post-tax-transfer): green ≤ 0.30; yellow 0.30 to 0.40; red > 0.40 sustained.
- Top-decile income share: green ≤ 25%; yellow 25% to 35%; red > 35% sustained.
- Wealth concentration (top 1% share): green ≤ 20%; yellow 20% to 30%; red > 30% sustained.

### Wellbeing

- Healthy life expectancy (year 50): green ≥ 75; yellow 70 to 75; red < 70.
- Loneliness rate (adults): green ≤ 12%; yellow 12% to 20%; red > 20%.
- Trust in institutions index: green ≥ 0.6; yellow 0.4 to 0.6; red < 0.4 sustained.
- Subjective wellbeing trend: green stable or rising; yellow modest decline; red sustained decline.

### Health

- Mental-health treatment access (urgent within 1 day): green ≥ 95%; yellow 80% to 95%; red < 80%.
- Suicide rate (per 100k): green stable or declining; yellow modest increase; red sustained increase or above 15.
- Preventable mortality: green declining; yellow stable; red rising.

### Education

- Upper-secondary completion: green ≥ 95%; yellow 85% to 95%; red < 85%.
- Adult literacy and numeracy at OECD high tier: green; OECD mid tier: yellow; below OECD mid tier: red.
- Inter-generational mobility (rank correlation): green low correlation (i.e., high mobility); red high correlation.

### Governance and Rights

- Rights-violation rate (per 100k): green ≤ 50; yellow 50 to 200; red > 200.
- Procedural fairness perceptions: green high; yellow medium; red low or falling.
- Recall and removal mechanisms: green operational and used; red captured or unused for cause.

### Ecology

- GHG emissions vs. budget: green on trajectory; yellow off trajectory; red sustained breach.
- Material footprint trend: green declining; red rising.
- Biodiversity intactness: green ≥ 0.85; yellow 0.7 to 0.85; red < 0.7.
- Water stress: green low; red high in any major watershed.

### Resilience

- Reserve durations meet ECN-IC2 targets: green; below 80% of target: yellow; below 50%: red.
- Recovery time after defined shock: green within targets; red beyond.

### Innovation

- New-firm rate: green stable or rising in non-financial sectors; red collapsing.
- Research-intensity: green above OECD median; red below.

### Care

- Caregiver burden distribution: green not concentrated; red highly concentrated by gender or ethnicity.
- Child wellbeing index: green high; red declining.

### Pluralism

- Discrimination-audit findings: green declining; red rising.
- Minority-rights audit: green passing; red failing.

### Observability

- Decision-log completeness: green ≥ 98%; yellow 90% to 98%; red < 90%.
- Audit-response rate: green high; red low.
- Observability-creep audit: green clean; red findings of personal-data surveillance.

## Scenario-Specific Criteria

For each scenario in ART-021, the framework passes if:

- No red lines breached.
- Critical adaptation criteria met.
- Indicator panel remains in green or yellow with documented response.
- Institutional mechanisms preserve their function.

The framework fails if:

- Any red line breached and not immediately corrected.
- Adaptation criteria missed.
- Multiple indicators move to red simultaneously.
- Trust in institutions collapses.

## Tradeoff Zones

Where two indicators move in opposite directions (yellow on one, green on another), the framework must declare the tradeoff explicitly and locate it in the constitutional conflict-resolution procedure (Article IV of ART-008). The simulation report identifies these zones; the decision log (ART-027) records how they were handled.

Documented tradeoff zones from this baseline:

- Privacy vs. effective surveillance for public health (TZ-004 + TZ-001).
- Innovation vs. ecological cap (TZ-007 via ECN-B1).
- Innovation vs. patent reform (ECO-P4 vs. innovation incentives).
- Subsidiarity vs. universal rights (TZ-006).
- Crisis efficacy vs. civil-liberties (TZ-001).
- Universal floor vs. inflation under stress (SCN-016).

## Redesign Triggers

The framework moves to active redesign (a new module-update or full-research iteration) if:

- Any red line is breached in ≥2 distinct scenarios with the same root cause.
- A single sub-module (governance body, regulation, mechanism) fails in ≥3 distinct scenarios.
- Compound scenarios produce coordinated failure across subsystems not predicted by single-scenario runs.
- An assumption in the assumption register (ART-028) is invalidated by simulation and an architecture module depended on it.
- A contradiction in the contradiction register (ART-029) is resolved in a way that requires re-spec of one or more modules.

## Falsification Conditions

The framework's core claims should be falsifiable. The following findings would falsify central claims:

- **Claim**: distributed authority resists capture.
  - **Falsifier**: scenarios SCN-001 and SCN-002 show consistent capture despite anti-capture mechanisms.
- **Claim**: sortition bodies are durable at scale.
  - **Falsifier**: SCN-019 shows sortition collapse or capture across most variations.
- **Claim**: universal floor + commons preserves dignity under shock.
  - **Falsifier**: SCN-003 and SCN-016 show floor erosion despite policy responses.
- **Claim**: hard ecological caps can be politically maintained.
  - **Falsifier**: SCN-005 with long-horizon shows cap-breaching as political-economy default.
- **Claim**: observability infrastructure does not become surveillance.
  - **Falsifier**: SCN-014 across most variations shows surveillance creep.
- **Claim**: emergency powers can be hard-limited.
  - **Falsifier**: SCN-012 shows ratchet effects across most variations.

If falsifiers obtain, the framework is materially weakened; the affected modules must be redesigned.

## Sensitivity Analysis

Sensitivity analyses for each scenario should identify:

- Which parameters move outcomes most.
- Which structural design choices are load-bearing.
- Which simplifying assumptions, if changed, change conclusions.

Reports must distinguish parameter sensitivity (calibration uncertainty) from structural sensitivity (design choice).

## False Precision and Reporting Discipline

Reports must:

- Use ranges, not point estimates, for forward projections.
- Report cross-model agreement separately from single-model results.
- Flag when results depend heavily on a single assumption.
- Refuse to advise on questions outside model validity.

This discipline is necessary because policy decisions taken from over-confident model output can do real harm (CLM-189, SIM-LIM6).

## Validation Report Format

Each iteration's `validation-report.md` (ART-023) reports against these criteria. The report must include:

- Pass/fail per scenario.
- Indicator panel outcomes.
- Red-line breaches (if any) with rationale.
- Sensitivity findings.
- Open issues raised by results.
- Recommended next iteration.

## Open Issues

- Thresholds in this artifact are illustrative; specific calibration depends on starting conditions and value-judgment about acceptable tolerance.
- Some red lines (constitutional court packed; election administration captured) are categorical and difficult to model precisely; require qualitative red-teaming alongside simulation.
- Compound-scenario reporting is more art than science at this maturity.
- Falsifiers (last section) are not necessarily mutually exclusive; a finding can simultaneously falsify several.
