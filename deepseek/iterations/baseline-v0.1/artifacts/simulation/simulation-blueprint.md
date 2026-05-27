# ART-019: Simulation Blueprint

Iteration: `baseline-v0.1`
Status: draft

## Purpose

Define how the civilization framework can be stress-tested through agent-based computational modeling, historical comparison, and scenario analysis. Specify model type, agent types, behavioral rules, institutional rules, resource flows, metrics, stress scenarios, validation thresholds, and known limitations.

## Model Type and Rationale

### Primary Approach: Agent-Based Modeling (ABM)

**Rationale**: The civilization framework is a complex adaptive system with heterogeneous agents, local interactions, emergent macro patterns, and non-linear dynamics. ABM is the natural modeling approach because:

1. It models individual agents with bounded rationality (BF-001)
2. It captures emergent institutional behavior from individual interactions
3. It enables heterogeneous agent populations (altruists, cooperators, defectors, etc.)
4. It supports multi-level analysis (individual, community, regional, national)
5. It allows parameter exploration and scenario testing without real-world experimentation

**Secondary Approaches**:
- **System Dynamics** for aggregate resource flows, ecological constraints, and demographic trends
- **Historical Comparative Analysis** for phenomena not easily modeled (cultural evolution, identity formation, narrative change)
- **Game-Theoretic Models** for specific institutional mechanisms (corruption dynamics, cooperation evolution)

### Simulation Framework Options

| Framework | Strengths | Weaknesses | Recommendation |
| --- | --- | --- | --- |
| NetLogo | Accessible, rapid prototyping, educational | Performance at scale, limited built-in analysis | Primary for prototype phase |
| Mesa (Python) | Python ecosystem, scalable, data-science integration | More setup overhead | Primary for production phase |
| Repast (Java/C++) | High performance, sophisticated features | Steep learning curve | Optional for high-performance needs |
| Custom ABM | Maximum flexibility | Maximum development cost | Not recommended for baseline |

**Decision**: Implement prototype in NetLogo for rapid iteration and visualization; production model in Mesa for integration with data-science pipelines (Python ecosystem). See ART-023 for framework recommendation.

---

## Agent Types

### Core Agent Types

| Agent Type | Description | Parameters |
| --- | --- | --- |
| Citizen | Individual person with needs, preferences, capabilities, and behaviors | Age, health status, education level, wealth, social capital, trust level, cooperation disposition (conditional cooperator, altruist, self-interested, defector), risk tolerance, time preference, civic engagement |
| Household | Group of cohabiting citizens sharing resources | Composition, shared wealth, care burden, consumption patterns |
| Community Cell | 100-300 households in geographic proximity, shared governance and infrastructure | Population, social capital, trust, cooperation norms, institutional quality, resource production, resilience capacity |
| Firm/Enterprise | Economic production unit. Can be cooperative, conventional, or public | Type, size, productivity, wages, environmental impact, governance structure |
| Government Institution | Regional or national governance body | Tier, competence, corruption level, capture risk, legitimacy, resource allocation |
| Natural Resource | Ecological asset (forest, water body, soil, biodiversity) | Stock, regeneration rate, carrying capacity, extraction rate, degradation status |

### Agent Heterogeneity

Agents are initialized with heterogeneous parameters drawn from specified distributions:
- Cooperation disposition: 50% conditional cooperator, 20% altruist, 5% unconditional cooperator, 15% self-interested, 10% defector (baseline assumption; adjustable parameter)
- Initial wealth: Gini coefficient ~0.35 (typical OECD) or ~0.45 (typical US) as baseline scenarios
- Risk tolerance, time preference, trust level: normal distributions with bounds

---

## Behavioral Rules

### Citizen Decision-Making

Agents follow bounded-rationality decision process (BF-001):
1. Perceive local environment (neighbors, institutions, resource availability)
2. Evaluate options against utility function with social preferences
3. Choose action with highest expected utility, probability-weighted by exploration factor
4. Update beliefs based on outcomes (reinforcement learning simple model)

### Cooperation Rules (BF-002, BF-003)
- Cooperate in common-pool resource use proportionally to: (a) observed cooperation of others, (b) trust in institutions, (c) perceived fairness of distribution, (d) detection probability of free-riding
- Defect when: (a) others defecting, (b) institutions perceived as unfair, (c) detection probability low, (d) resource scarcity acute (survival override)
- Trust updates: trust increases when institutions deliver on promises; trust decreases rapidly when institutions fail

### Economic Behavior
- Work effort function: intrinsic (autonomy, competence, relatedness per BF-005) + extrinsic (compensation, security)
- Consumption: basic needs first, then positional goods (BF-011), then savings, then luxury
- Investment: cooperative enterprises reinvest in community; conventional firms maximize profit; public enterprises balance profit and public good
- Innovation: random-walk with fitness selection; rate depends on education investment and cooperative/competitive dynamics

### Civic Participation
- Voting: probability proportional to (civic education * trust in institutions * perceived efficacy)
- Community participation: probability proportional to (social capital * time availability * community satisfaction)
- Corruption: probability proportional to (power * detection probability * moral weight)
- Emigration: probability proportional to (dissatisfaction - exit costs)

---

## Institutional Rules

### Governance Institutions (per ART-009)
- Tier-1 (Community): agents deliberate, vote, implement community projects. Sortition for council positions.
- Tier-2 (Regional): agents represented through electoral + sortition + expert. Resource allocation, infrastructure investment, dispute resolution.
- Tier-3 (National): agents represented through electoral + sortition + expert. Constitutional enforcement, defense, currency.

### Institutional Quality Dynamics
- Institutional quality = f(initial design, resources, corruption, citizen engagement, external shocks)
- Corruption spreads through agent networks with probability proportional to institutional weakness and detection probability (RSK-004)
- Institutional capture modeled as wealthy agents purchasing policy influence, with probability proportional to inequality and inversely proportional to anti-corruption mechanisms

### Economic System (per ART-010)
- Commons layer: universal services funded through progressive taxation; service quality declines if tax base shrinks
- Cooperative layer: worker-owned enterprises; profit-sharing; employment stability (wage reduction instead of layoffs)
- Entrepreneurial layer: competitive market with anti-monopoly constraints
- Tax system: progressive income + wealth + LVT + ecological + inheritance

### Ecological System (per ART-015)
- Resource stocks with regeneration rates and carrying capacities
- Extraction by human agents; pollution as byproduct of production
- Planetary boundaries as hard constraints: violation triggers automatic policy response
- Ecological tipping points: irreversible state transitions when certain thresholds crossed

---

## Resource Flows

### Material Flows
- **Food**: Production (farms, gardens) -> Distribution -> Consumption -> Waste -> Compost/return
- **Energy**: Generation (renewable) -> Storage -> Distribution -> Consumption
- **Water**: Sources -> Treatment -> Distribution -> Consumption -> Treatment -> Return
- **Materials**: Extraction/Import -> Manufacturing -> Use -> Reuse/Repair -> Recycling -> Disposal

### Financial Flows
- **Taxation**: Citizens/Enterprises -> Government -> Public Services/Transfers
- **Wages/Profits**: Enterprises -> Citizens (with cooperative/conventional/investor distribution rules)
- **Investment**: Savings -> Financial System -> Enterprise Investment
- **Commons funding**: Tax Revenue -> Universal Services -> Universal Access

### Information Flows
- **Observability**: Institutional Processes -> Public Dashboard -> Citizen Awareness -> Trust Update
- **Misinformation**: External/Domestic Sources -> Agent Belief Update -> Trust Update -> Cooperation Update
- **Education**: Schools -> Knowledge Transfer -> Civic Competence -> Participation

---

## Metrics (also feed ART-020 model-parameters.yaml)

### Wellbeing Metrics
- Subjective Wellbeing (happiness/life-satisfaction score -- individual agent variable)
- Multidimensional Wellbeing Index (health, education, income, social connection, safety, environment)
- Gini coefficient (income, wealth)
- Poverty rate (% below basic-needs threshold)
- Health-adjusted life expectancy

### Institutional Metrics
- Trust in institutions (% agents above trust threshold)
- Institutional quality score (composite of competence, fairness, transparency)
- Corruption index (corrupt transactions / total transactions)
- Participation rate (% agents voting, community-engaged)
- Democratic-backsliding index (institutional quality trend)
- Capture risk index (wealth-concentration * institutional weakness)
- Observability coverage (% institutional processes visible to members)

### Ecological Metrics
- Carbon emissions (cumulative, annual rate)
- Biodiversity index (species richness relative to baseline)
- Resource-depletion rate (% of renewable resources consumed relative to regeneration)
- Material footprint per capita
- Planetary-boundary transgression count (0-9 boundaries)

### Resilience Metrics
- Recovery time from shocks (time to 90% pre-shock function)
- Cascading-failure propagation (nodes affected over time)
- Trust-recovery rate (post-shock trust trajectory)
- Food/energy/water self-sufficiency duration

### Economic Metrics
- GPI (Genuine Progress Indicator)
- GDP (for comparison with legacy metrics)
- Employment rate
- Innovation rate (patents, enterprise creation, productivity growth)
- Care-economy contribution (measured and recognized)
- Commons-layer service quality

---

## Stress Scenarios (detailed in ART-021)

| Scenario | Trigger | Key Parameters Varied |
| --- | --- | --- |
| SCN-001: Elite Capture | Wealth concentration increases; campaign-finance rules weakened | Inequality, corruption rate, institutional quality |
| SCN-002: Ecological Overshoot | Resource consumption exceeds regeneration | Resource stock, pollution, policy response delay |
| SCN-003: Democratic Backsliding | Populist leader elected; institutional norms eroded | Trust, institutional quality, emergency-powers abuse |
| SCN-004: Economic Shock | External trade disruption; financial crisis | GDP, unemployment, inequality, trust, cooperation |
| SCN-005: External Military Threat | Neighboring hostile power; conventional threat | Defense spending, civil-defense mobilization, rights tradeoffs |
| SCN-006: Pandemic | Novel pathogen with various severity/transmissibility | Healthcare capacity, mortality, economic disruption, trust |
| SCN-007: AI Disruption | Rapid automation of 30-50% of jobs | Employment, inequality, reskilling effectiveness, UBS adequacy |
| SCN-008: Information Collapse | Coordinated disinformation campaign | Trust, polarization, cooperation, institutional legitimacy |
| SCN-009: Generational Drift | Civic commitment declines over 2-3 generations | Civic engagement, institutional quality, cultural transmission |
| SCN-010: Cascading Compound Crisis | Multiple scenarios simultaneously (ecological + economic + political) | All parameters stressed simultaneously |

---

## Validation Thresholds (detailed in ART-022)

### Green Zone (Design Validated)
- All wellbeing metrics improve or remain stable over 100-year simulation
- Gini coefficient below 0.35
- Trust in institutions above 60%
- Planetary boundaries maintained (or returning toward safe zone)
- Corruption index below 10% baseline
- Recovery from major shocks within 5 years

### Yellow Zone (Design Requires Adjustment)
- Any wellbeing metric declines >10% over 50 years
- Gini coefficient exceeds 0.40
- Trust falls below 50%
- One or more planetary boundaries transgressed
- Corruption index exceeds 15%
- Recovery from shock exceeds 10 years

### Red Zone (Design Failure -- Redesign Required)
- Any wellbeing metric declines >25% over 50 years
- Systemic collapse (population decline, institutional failure cascade)
- Gini exceeds 0.50
- Trust falls below 30%
- Multiple planetary boundaries transgressed with irreversible tipping points
- Democratic backsliding to authoritarian threshold
- Shock recovery exceeding 25 years or never recovering

---

## Model Limitations (Must Report)

1. **Abstraction gap**: Any computational model abstracts away complexity. Many factors (culture, identity, narrative, charisma, technological breakthroughs) cannot be adequately modeled.

2. **Parameter uncertainty**: Many parameters are estimated or assumed. Sensitivity analysis must report which parameters drive results.

3. **Emergence unpredictability**: Complex adaptive systems produce emergent behaviors not predictable from agent rules alone. Model results are exploratory, not predictive.

4. **Equilibrium assumptions**: Some behaviors may only manifest in long-run equilibrium; models with finite runtime may miss these.

5. **Calibration data scarcity**: No existing civilization matches this framework for calibration. Parameters derived from analogies (Nordic model, Swiss confederation, Mondragon) may not transfer.

6. **Black swan events**: Tail-risk events (RSK-018 nuclear/existential catastrophe) cannot be adequately modeled.

7. **Value conflicts**: Some value tradeoffs are normative (CON-VAL-001 through CON-VAL-007) and cannot be resolved by simulation.

8. **Implementation transition**: Static parameter initialization does not capture transition dynamics from existing institutions to framework architecture.

9. **Cultural and historical specificity**: Behavioral assumptions drawn primarily from WEIRD populations (BF-008). Cross-cultural validity of behavioral parameters is uncertain.

10. **Simplified agent psychology**: Agents follow simplified decision rules. Real human behavior includes narrative, identity, meaning-making, and non-rational motivations that ABM cannot capture.

---

## Known Model Limitations (additional to above)

| Limitation | Severity | Mitigation |
| --- | --- | --- |
| Cultural evolution not modeled | High | Supplement with historical comparative analysis |
| Technology innovation path not predictable | High | Scenario-based rather than predictive modeling |
| Agent value-learning not implemented | Medium | Parameter sweeps across value-weight variations |
| Intergenerational value transmission simplified | Medium | Agent reproduction with partial cultural inheritance |
| External geopolitical environment assumed stable | High | Scenario modeling of external-shock scenarios |
| Information ecosystem simplified | Medium | Add misinformation-agent type in future iteration |
| Network effects on behavior simplified | Medium | Implement spatial/social-network topology in production phase |
| Mental health as agent state underspecified | Medium | Add wellbeing and trauma parameters in future iteration |