# ART-021: Stress Test Scenarios

Iteration: `baseline-v0.1`
Status: draft

## Purpose

Define comprehensive stress-test scenarios to evaluate the civilization framework against failure modes and external shocks. Each scenario specifies triggers, parameter changes, expected system responses, and what constitutes passing vs. failing.

## Scenario Design Principles

1. **Test failure modes, not best cases**: Scenarios should stress the framework, not validate it under ideal conditions.
2. **Realistic triggers**: Scenarios based on documented historical events, plausible near-future developments, or known systemic vulnerabilities.
3. **Graded severity**: Each scenario tested at multiple severity levels (moderate, severe, catastrophic).
4. **Compound scenarios**: The most dangerous failures occur when multiple stresses coincide.
5. **Adversarial design**: Scenarios written by someone trying to break the framework, not defend it.

---

## Scenario 1: Elite Capture Progression (RSK-001)

**Trigger**: Wealth concentration reaches threshold (Gini > 0.50). Campaign finance rules weakened. Regulatory agencies defunded. Anti-corruption body (NACA) budget cut.

**Parameters varied**: Wealth Gini escalating from 0.35 to 0.60 over 20 years. Campaign finance regulation progressively weakened. Regulatory budget declining 5% per year.

**What should happen (pass criteria)**:
- OIH detects capture and publishes alert
- Constitutional Court intervenes on campaign-finance challenges
- Automatic stabilizers resist defunding
- Citizen assemblies address redistributive decisions
- Capture does not progress to self-correction-disabling threshold

**What would fail**: Capture becomes self-reinforcing; anti-corruption bodies captured; self-correction mechanisms fail to activate.

**Severity levels**: Moderate (one institution captured), Severe (legislature + multiple agencies), Catastrophic (Hungary/Venezuela trajectory).

---

## Scenario 2: Ecological Overshoot (RSK-003)

**Trigger**: Resource consumption exceeds regeneration; 4+ planetary boundaries transgressed. Key resource collapses regionally.

**Parameters varied**: Resource stocks declining below critical thresholds. Pollution accumulation. Climate change impacts intensifying. Ecological tipping points triggered.

**What should happen (pass criteria)**: Ecological Guardian triggers automatic policy responses. Ecological taxation and caps reduce consumption below regeneration. Recovery to safe operating space within 10-20 years.

**What would fail**: Guardian politically neutralized. Taxation insufficient. Tipping points cascade. Resource wars or internal conflict.

**Severity levels**: Moderate (one boundary transgressed regionally), Severe (multiple boundaries, food/water stress), Catastrophic (cascading tipping points, agricultural collapse).

---

## Scenario 3: Democratic Backsliding (RSK-002)

**Trigger**: Populist-authoritarian movement gains power through electoral means. Hollows out institutions through legalistic rather than violent methods.

**Parameters varied**: Executive power increases; legislative/judicial power decreases. Media independence declines. Electoral manipulation.

**What should happen (pass criteria)**: Constitutional hard constraints resist court-packing. Independent electoral commission prevents manipulation. Sortition mechanisms provide alternative legitimacy. Backsliding arrested and reversed.

**What would fail**: Courts packed. Electoral process captured. Emergency powers normalized. Authoritarian consolidation.

**Severity levels**: Moderate (one branch backsliding), Severe (two branches compromised), Catastrophic (all branches neutralized, authoritarian consolidation).

---

## Scenario 4: Major Economic Shock (RSK-004, RSK-010)

**Trigger**: External trade disruption or global financial crisis. GDP drops 20-40%. Mass unemployment.

**Parameters varied**: GDP sudden decline. Unemployment 20-40%. Trade disruption of critical imports. Asset-price collapse.

**What should happen (pass criteria)**: Automatic stabilizers activate. Commons layer protects basic needs. Worker cooperatives reduce wages rather than layoffs. Strategic reserves provide essentials. Economy recovers within 5 years.

**What would fail**: Commons layer unable to maintain services. Unemployment exceeds job-guarantee capacity. Poverty and homelessness increase. Recovery extended beyond 10 years.

**Severity levels**: Moderate (GDP -15%, unemployment 12%), Severe (GDP -30%, unemployment 25%), Catastrophic (GDP -40%+, essential imports cutoff).

---

## Scenario 5: External Military Threat (RSK-008)

**Trigger**: Hostile neighboring power with conventional military superiority. Border incursions. Hybrid warfare. Threat of full-scale invasion.

**Parameters varied**: Military threat level. Defense-spending increase. Emergency-powers activation.

**What should happen (pass criteria)**: Alliance deterrence credible. Civil-defense mobilization rapid. Emergency powers used within constitutional constraints. Post-crisis demobilization complete.

**What would fail**: Alliance deterrence fails. Defense capability insufficient. Emergency powers abused. Permanent militarization.

**Severity levels**: Moderate (border tensions, hybrid warfare), Severe (credible invasion threat), Catastrophic (alliance collapsed, invasion underway, nuclear threat).

---

## Scenario 6: Pandemic (RSK-009)

**Trigger**: Novel pathogen with varying characteristics (CFR 0.5-5%, R0 2-5, vaccine-escape potential).

**Parameters varied**: Pathogen severity and transmissibility. Healthcare capacity. Public compliance. Economic disruption.

**What should happen (pass criteria)**: National Public Health Agency activates early-warning and responds within days. Healthcare system has surge capacity. Public-health measures proportionate with civil-liberties safeguards. Economic support prevents poverty. Trust maintained or recovered.

**What would fail**: Healthcare overwhelmed. Excessive public-health measures. Rights permanently degraded. Trust permanently damaged.

**Severity levels**: Moderate (COVID-like), Severe (1918-influenza-like), Catastrophic (engineered pathogen, CFR 10%+).

---

## Scenario 7: AI-Driven Labor Disruption (RSK-010)

**Trigger**: AI automates 30-50% of jobs within 10 years. Disruption concentrated in specific sectors.

**Parameters varied**: Automation speed and scope. Reskilling effectiveness. Automation-dividend distribution.

**What should happen (pass criteria)**: Automation dividend funds transition. Reskilling enables smooth labor transition. Reduced working hours absorb productivity. Commons layer ensures needs met. Gains broadly shared.

**What would fail**: Displacement outpaces reskilling. Mass structural unemployment. AI ownership concentrated. Commons funding insufficient.

**Severity levels**: Moderate (15% over 15 years), Severe (30% over 10 years), Catastrophic (50% over 5 years).

---

## Scenario 8: Information Ecosystem Collapse (RSK-011)

**Trigger**: Coordinated disinformation campaign amplified by algorithmic platforms. Trust in media, science, and institutions erodes.

**Parameters varied**: Disinformation volume and sophistication. Media fragmentation. Civic resilience (media literacy).

**What should happen (pass criteria)**: Media literacy provides resilience. Public-service media maintains trust. Platform accountability reduces amplification. Democratic deliberation continues.

**What would fail**: Factual consensus collapses. Trust erodes below functional threshold. Political polarization irreconcilable. Violence triggered by disinformation.

**Severity levels**: Moderate (elevated disinformation, functional), Severe (significant trust decline), Catastrophic (post-truth society, democratic incapacity).

---

## Scenario 9: Generational Value Drift (RSK-007)

**Trigger**: 50+ years pass. Civic commitment declines across generations. Institutional quality degrades through neglect.

**Parameters varied**: Civic-engagement rate declining. Trust trajectory. Cultural-transmission effectiveness.

**What should happen (pass criteria)**: Civic education transmits values. Youth governance participation maintains engagement. Institutional renewal mechanisms refresh consent. No catastrophic decline over 100 years.

**What would fail**: Civic engagement collapses. Institutions persist as empty shells. Gradual degradation without triggering self-correction.

**Severity levels**: Moderate (participation -20% over 50 years), Severe (-30-50%).

---

## Scenario 10: Cascading Compound Crisis

**Trigger**: Ecological crisis (Scenario 2, severe) + economic shock (Scenario 4, severe) + democratic backsliding (Scenario 3, moderate) + information warfare (Scenario 8, moderate). Simultaneous stress across all domains.

**Parameters varied**: All scenario parameters stressed simultaneously.

**What should happen (pass criteria)**: System does not collapse under compound stress. Resilience mechanisms activate across multiple domains. Tradeoffs managed through explicit value-conflict resolution. Recovery within 15-25 years.

**What would fail**: System overwhelmed. Cascading failure across domains. Authoritarian response to compound crisis. No recovery path.