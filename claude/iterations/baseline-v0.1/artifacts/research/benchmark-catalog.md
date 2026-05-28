# Benchmark Catalog

Artifact ID: ART-005
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: MOD-RES
Depends on: ART-003, ART-004

## Purpose

Catalog of historical civilizations, intentional communities, and modern polities that this iteration draws on as design references. Each entry records: what the system reportedly did, mechanisms that plausibly contributed, durability, known failure conditions, and which design lessons transfer with what caveats. Inclusion is not endorsement; cataloging contested cases lets later iterations argue the transfer explicitly.

## Format

Each benchmark entry uses this structure:

- **ID and name**: stable identifier and common name.
- **Era and scale**: rough dates and population scope.
- **Mechanisms of interest**: what about the case is worth design attention.
- **Apparent durability**: how long the relevant features persisted.
- **Failure or limit conditions**: what eventually constrained or ended them.
- **Transferable lessons**: candidate design implications for this framework.
- **Caveats**: selection bias, source quality, romanticization risk, non-transferability factors.
- **Source IDs**: from `source-register.md`.

## A. Historical Civilizations and Polities

### BMK-001 Roman Republic (institutional design phase)

- Era and scale: roughly 509 BCE - 27 BCE; peak governance population in the low millions of citizens, larger total subject population.
- Mechanisms of interest: separation of powers across consuls, Senate, and assemblies; annual rotation of executive office; checks against single-person tyranny through dual consulship and tribunician veto; gradual incorporation of new groups into political community (with limits).
- Apparent durability: roughly 480 years before transition to principate; institutional forms persisted in altered shape much longer.
- Failure conditions: military expansion outpaced civic institutions; client armies loyal to commanders rather than republic; entrenched land inequality; political violence normalization; failure to adapt institutions to scale.
- Transferable lessons: rotation, dual executive, multi-body check architecture, gradual citizenship extension; warning that external expansion and internal inequality can co-erode republican forms.
- Caveats: slave economy and gendered exclusion are part of the case; "transferable lessons" must be extracted without romanticization. Causal interpretations of collapse are contested.
- Source IDs: SRC-001, SRC-009.

### BMK-002 Byzantine Empire (Eastern Roman continuation)

- Era and scale: roughly 330 CE - 1453 CE; multi-millions across changing geography.
- Mechanisms of interest: durable bureaucratic state with codified law (Justinian's Corpus Juris Civilis); sustained military-fiscal apparatus; adaptive diplomacy; institutional continuity across dynastic changes.
- Apparent durability: over 1,100 years from Constantinople's founding.
- Failure conditions: chronic external pressure on multiple fronts, fiscal exhaustion, theological-political fragmentation, eventual military overmatch.
- Transferable lessons: codified administrative law and continuous bureaucracy can outlast charismatic leadership; diplomacy and selective alliance is part of resilience.
- Caveats: imperial, hierarchical, theocratic; selective extraction of institutional patterns is required.
- Source IDs: SRC-009, SRC-010.

### BMK-003 Iroquois (Haudenosaunee) Confederacy

- Era and scale: roughly 12th-16th century formation through 18th century; tens of thousands across constituent nations.
- Mechanisms of interest: consensus-based council with clan-based representation; clan mothers' authority over chiefs; the Great Law of Peace as a written constitution; explicit conflict-resolution and peacekeeping procedures; intergenerational ("seven generations") decision standard.
- Apparent durability: core institutional structure persisted across centuries despite displacement and treaty violations.
- Failure conditions: external colonial pressure, disease, displacement; not internal collapse.
- Transferable lessons: long-horizon decision standards; clan/gender-balanced authority; codified peace-making procedures; nested governance.
- Caveats: do not abstract away from indigenous sovereignty and the specific cultural matrix; do not appropriate ceremony.
- Source IDs: SRC-075, SRC-074.

### BMK-004 Swiss Confederation

- Era and scale: 1291 origin through present; current population roughly 9 million.
- Mechanisms of interest: cantonal sovereignty with confederal coordination; direct-democratic instruments (initiatives, referenda); militia-based defense; multilingual and multireligious cohabitation; long-term neutrality; budgetary discipline.
- Apparent durability: continuous federal arrangement under varying forms for centuries.
- Failure conditions: limits include slow expansion of voting rights (women's suffrage federally only in 1971), structural tensions in immigration policy.
- Transferable lessons: federalism with strong local fiscal autonomy; direct-democratic instruments as legitimacy reinforcement; militia / civil defense models; consensus executive (Federal Council).
- Caveats: small scale and geographic protection; selection effects make direct comparison to large states risky.
- Source IDs: SRC-051, SRC-053.

### BMK-005 Nordic Social Democracies (Sweden, Denmark, Norway, Finland, Iceland)

- Era and scale: late 19th century origins, mature form mid-20th century to present; populations from roughly 300,000 (Iceland) to 10 million (Sweden).
- Mechanisms of interest: universal public services; high but transparent taxation; active labor market policies; tripartite labor-employer-state bargaining; high union density; gender-egalitarian family policy; strong measurement of social outcomes; consensus political culture.
- Apparent durability: institutional core stable for several decades through political alternation.
- Failure conditions: vulnerability to capital mobility, demographic transition, immigration-policy strain, inequality drift since the 1990s, climate-policy tension.
- Transferable lessons: universal services as legitimacy anchor; data-rich public administration; labor-market institutions matter; gender-equitable care infrastructure.
- Caveats: small homogeneous populations and resource endowments are part of the explanation; scale and heterogeneity translation is non-trivial.
- Source IDs: SRC-020, SRC-087, SRC-102.

### BMK-006 Singapore

- Era and scale: 1965 independence to present; about 6 million.
- Mechanisms of interest: meritocratic civil service with high pay and strict accountability; long-term planning bureaucracy; public housing scale (over 80 percent of residents); ethnic-mix policies in housing; strict rule of law; aggressive anti-corruption enforcement; sovereign-wealth investment; multi-language education.
- Apparent durability: roughly six decades of sustained per-capita growth and institutional continuity.
- Failure conditions / limits: limited political pluralism; constrained civil society; vulnerability to external trade shocks; demographic decline.
- Transferable lessons: well-paid, accountable civil service; long-term planning capacity; housing as policy lever; civic-language norms with multi-ethnic protections.
- Caveats: city-state scale; semi-authoritarian governance is structurally entwined with the success story; lessons must be carefully decoupled.
- Source IDs: SRC-002, SRC-051.

### BMK-007 Costa Rica

- Era and scale: 1948 abolition of standing army to present; about 5 million.
- Mechanisms of interest: constitutional abolition of military, with budget redirection to health and education; durable democracy with high voter participation; payments-for-ecosystem-services policies; reforestation reversal of mid-century deforestation.
- Apparent durability: over 75 years of demilitarized democracy.
- Failure conditions / limits: small economy; reliance on tourism and foreign investment; inequality drift; security-spending pressure from regional crime.
- Transferable lessons: constitutional demilitarization is feasible at small scale with regional security guarantees; ecological payment systems can shift land-use trajectories.
- Caveats: geographic and regional-political conditions are part of the story; not generalizable to states with hostile borders.
- Source IDs: SRC-051, SRC-052.

### BMK-008 Uruguay

- Era and scale: 20th century social-policy phase to present; about 3.4 million.
- Mechanisms of interest: early universal welfare-state construction in Latin America; durable secular democracy; high social trust; cannabis and other regulated-market policy experiments; well-developed labor institutions.
- Apparent durability: institutional core re-established after 1985 democratic transition and durable since.
- Failure conditions / limits: persistent fiscal pressure; regional macro spillovers; demographic aging.
- Transferable lessons: early welfare-state institutionalization shapes long trajectories; regulated-market experiments can be conducted without civil-liberties collapse.
- Caveats: small homogeneous population by Latin American standards.
- Source IDs: SRC-087, SRC-051.

### BMK-009 South Korea (post-1987 democratic period)

- Era and scale: 1987 democratization to present; about 51 million.
- Mechanisms of interest: rapid industrial development, then democratic transition; high educational investment; public-broadcasting and judicial reform; anti-corruption prosecutions of former presidents; strong administrative capacity.
- Apparent durability: roughly four decades of democratic institutional life; durable rule of law.
- Failure conditions / limits: chaebol economic concentration; demographic decline; gender inequality; mental-health stressors; geopolitical risk.
- Transferable lessons: democratic accountability can succeed in a developmental state after transition; education investment compounds; judicial independence is reachable through reform.
- Caveats: developmental-state context not transferable to mature post-industrial settings.
- Source IDs: SRC-051, SRC-052.

### BMK-010 Tokugawa Japan (Edo period stable phase)

- Era and scale: 1603-1868; roughly 30 million by late period.
- Mechanisms of interest: long internal peace; strict bureaucratic stratification; intricate urban planning; resource constraint management (forest policy); cultural and intellectual flourishing within constraints.
- Apparent durability: roughly 265 years of internal peace.
- Failure conditions: rigidity to external shock; collapse under modern-state contact pressure.
- Transferable lessons: resource-cycling and population-stability practices can be sustained for centuries when institutional rules align; warning that internal stability without adaptive capacity becomes brittleness.
- Caveats: rigid stratification and external isolation are part of the package; lessons must be extracted carefully.
- Source IDs: SRC-001, SRC-064.

### BMK-011 Roman Empire (failure case)

- Era and scale: 27 BCE - 476 CE (West); peak population perhaps 60 million.
- Mechanisms of interest: scale of administrative reach; legal codification; engineering infrastructure; military-fiscal complex.
- Apparent durability: roughly 500 years in the West.
- Failure conditions: fiscal exhaustion, currency debasement, military-political fusion, succession crises, climate stress, plague, migration pressure, ideological fragmentation.
- Transferable lessons: large administrative states fail through compounding stressors, not single causes; military-political fusion is dangerous; legal codification is a long-run asset.
- Caveats: the case is in the failure-mode register; included here for institutional benchmarks.
- Source IDs: SRC-001, SRC-002.

### BMK-012 Soviet Union (failure case)

- Era and scale: 1922-1991; over 280 million at peak.
- Mechanisms of interest: planning bureaucracy; mass literacy and industrialization; universal services; militarized civil defense.
- Apparent durability: roughly 70 years.
- Failure conditions: economic information failure under central planning; political legitimacy erosion; ethnic and federal tensions; cost of military competition; rigid succession; suppression of feedback.
- Transferable lessons: feedback suppression is catastrophic; planning without market or commons feedback fails on complex consumption; universal-services lessons survive ideological framing.
- Caveats: do not extract socio-political features without their authoritarian context.
- Source IDs: SRC-001, SRC-002, SRC-011.

### BMK-013 Weimar Republic (collapse case)

- Era and scale: 1919-1933; about 60 million.
- Mechanisms of interest: democratic constitutional design with proportional representation; emergency powers (Article 48); economic shock vulnerability.
- Apparent durability: 14 years.
- Failure conditions: hyperinflation, depression, polarization, paramilitarization, executive emergency-power overuse, normalization of anti-democratic actors.
- Transferable lessons: emergency-power abuse pathway; need for cordon sanitaire against anti-democratic actors; institutional resilience to economic shock matters.
- Caveats: historical and ideological specificity; pattern is general but specifics are not.
- Source IDs: SRC-011.

## B. Intentional Communities and Cooperative Experiments

### BMK-020 Mondragon Cooperative Corporation

- Era and scale: founded 1956 in Basque region; tens of thousands of worker-members across many cooperatives.
- Mechanisms of interest: federated cooperative model; internal solidarity fund; capped pay ratios within firms; cooperative bank financing; education-cooperative pipeline.
- Apparent durability: roughly 70 years across multiple economic cycles.
- Failure conditions / limits: pay-ratio drift over time; subsidiary firms partly outside cooperative discipline; failure of Fagor Electrodomesticos (2013).
- Transferable lessons: federation of cooperatives can scale beyond firm level; internal capital institutions matter; pay-ratio drift requires explicit defense.
- Caveats: regional culture and historical conditions partly explain durability.
- Source IDs: SRC-017, SRC-018.

### BMK-021 Kibbutz Movement (early and reformed phases)

- Era and scale: roughly 1909 to present; many tens of thousands of members at peak.
- Mechanisms of interest: collective ownership and labor; egalitarian wage schemes; communal childrearing (early phase); democratic assemblies; defense participation.
- Apparent durability: long-running but with substantial reform from the 1990s onward (privatization waves).
- Failure conditions / limits: external economic pressure; generational withdrawal; equality versus individual incentive tensions.
- Transferable lessons: collective economic forms are sustainable when paired with strong identity and external supports; equality-versus-incentive design tensions are real.
- Caveats: specific cultural and security context.
- Source IDs: SRC-051, SRC-053.

### BMK-022 Auroville (Tamil Nadu, India)

- Era and scale: founded 1968; population in the low thousands.
- Mechanisms of interest: explicit experimental governance; unity through diversity; non-currency internal economy attempts; ecological restoration of a degraded landscape.
- Apparent durability: roughly 55 years; intermittent governance crises and recent state-intervention episodes.
- Failure conditions / limits: small scale; conflict over authority and external state relations.
- Transferable lessons: durable ecological restoration is possible; voluntary commons need external legal recognition to avoid capture.
- Caveats: small intentional-community context; not directly scalable.
- Source IDs: SRC-075.

### BMK-023 Twin Oaks (Virginia, US)

- Era and scale: founded 1967; about 90 members typical.
- Mechanisms of interest: income-sharing community; labor-credit system; consensus governance with formal procedures; partial economic self-sufficiency.
- Apparent durability: over 55 years.
- Failure conditions / limits: small scale; selection effects on members.
- Transferable lessons: labor-credit accounting can substitute for wage labor at small scale; consensus governance needs explicit procedure.
- Caveats: scale-bounded; voluntary entry and exit are critical.
- Source IDs: SRC-006.

### BMK-024 Open-source software commons (Linux kernel, Wikipedia, etc.)

- Era and scale: late 20th century to present; global distributed participation.
- Mechanisms of interest: meritocratic contribution norms; modular technical architecture; explicit governance bodies; license-based commons protection; reputation-based authority.
- Apparent durability: multiple decades across projects.
- Failure conditions / limits: maintenance under-funding; bus-factor risk; capture by corporate interests in dependent ecosystems; harassment dynamics in some communities.
- Transferable lessons: digital commons can be governed durably with explicit licensing and modular technical design; long-term maintenance funding is a known design gap.
- Caveats: digital commons differ from physical-resource commons; not all features transfer.
- Source IDs: SRC-006, SRC-053.

## C. Sector-Specific Benchmark Programs

### BMK-030 Universal-coverage public health systems (UK NHS, French SS, Taiwan NHI, Costa Rica CCSS)

- Mechanisms of interest: single-payer or near-universal coverage with different financing mixes; primary-care anchoring; cost control mechanisms; population-health measurement.
- Lessons: universal coverage is operationally feasible at very different income levels; cost control is the chronic challenge; primary-care anchoring outperforms specialty-led systems on aggregate health.
- Caveats: outcomes depend heavily on continuous political-financial support and on social determinants outside health systems.
- Source IDs: SRC-023, SRC-055.

### BMK-031 High-performing school systems (Finland, Singapore, Estonia, parts of Canada)

- Mechanisms of interest: high teacher status and selection; equity in resource distribution; moderate standardized assessment intensity (Finland) or high-intensity systems with strong supports (Singapore); strong digital infrastructure (Estonia).
- Lessons: multiple distinct designs achieve high outcomes; common factors include resource equity, teacher quality, and aligned curriculum.
- Caveats: cultural and social conditions co-vary with school-system features.
- Source IDs: SRC-028, SRC-031.

### BMK-032 Participatory-budgeting cases (Porto Alegre and adaptations)

- Mechanisms of interest: structured citizen deliberation over capital budget allocation; multi-year processes; equity weighting.
- Lessons: participatory mechanisms can shift expenditure toward under-served areas; durability depends on political-leadership continuity.
- Caveats: most successful replications are smaller-scale; outcomes mixed where the political environment shifted.
- Source IDs: SRC-088.

### BMK-033 Citizens' assemblies (Ireland, France, Iceland, UK climate assembly)

- Mechanisms of interest: randomly selected citizen panels deliberating on contested policy questions; expert input integrated; recommendations to legislatures.
- Lessons: deliberation under structured facilitation produces stable, often centrist recommendations on charged issues; durability depends on legislative uptake.
- Caveats: time-bounded; effect on durable policy adoption uneven.
- Source IDs: SRC-013, SRC-089.

### BMK-034 Sovereign wealth and pension funds (Norway GPFG, Alaska Permanent Fund, Singapore Temasek)

- Mechanisms of interest: rent capture from finite resources or strategic assets; long-horizon investment governance; transparency rules; per-citizen distribution (Alaska).
- Lessons: rent capture and long-horizon investment is feasible with strong governance; per-citizen distribution can co-exist with sovereign investment.
- Caveats: depends on initial resource or asset base; not portable to states without such bases.
- Source IDs: SRC-017, SRC-095.

### BMK-035 Bhutan Gross National Happiness framework

- Mechanisms of interest: composite well-being indicator embedded in policy review; multidimensional poverty index applied at national level.
- Lessons: alternative-indicator regimes are administratively feasible; effectiveness depends on whether the composite shapes budgets.
- Caveats: small country; political environment shapes outcomes.
- Source IDs: SRC-018, SRC-097, SRC-098.

### BMK-036 Estonia digital state

- Mechanisms of interest: comprehensive digital public services; data-once principle; X-Road interoperability; transparent data-access logs; citizen control over personal data; strong cyber-resilience emphasis.
- Lessons: digital-state services and member observability of own data are jointly achievable; transparent access logs build trust.
- Caveats: small population; geopolitical context drove cyber-resilience investments; specific tradeoffs around centralized digital identity.
- Source IDs: SRC-077.

### BMK-037 Disaster preparedness systems (Japan, Cuba, New Zealand)

- Mechanisms of interest: drilled civilian response; redundant logistics; clear hierarchies during emergency with rapid reversion to normal authority.
- Lessons: anticipatory preparedness and clear, time-limited emergency authority outperform improvised response on outcomes.
- Caveats: cultural and institutional context affects compliance.
- Source IDs: SRC-064, SRC-038.

## D. Negative Examples (catalogued elsewhere, summarized here)

- Weimar (BMK-013), Late Roman Empire (BMK-011), USSR (BMK-012): documented in `failure-mode-register.md`.
- Modern democratic backsliding cases (Hungary, Turkey, Venezuela, others): see CLM-100 and SRC-011, SRC-051; treated structurally in `failure-mode-register.md` and `governance-system.md`.

## Lessons Synthesis

A small number of design lessons recur across benchmarks. None of these is a guarantee; each requires translation to scale and context.

1. **Distribute authority across multiple bodies and time-rotate it.** Roman Republic, Swiss Confederation, Iroquois Confederacy, Mondragon, citizens' assemblies all distribute and rotate authority.
2. **Pair codified rules with continuous bureaucratic capacity.** Byzantine Empire, Singapore, Nordics, Estonia all couple rules with capable administration.
3. **Couple universal services with measurable accountability.** Nordics, Costa Rica, universal-health-system cases (BMK-030).
4. **Build participatory institutions before crisis, not during.** Citizens' assemblies, participatory budgeting, Iroquois consensus all rely on standing practice.
5. **Treat ecological and resource constraints as structural, not external.** Tokugawa forest policy, sovereign-wealth rent capture, payments-for-ecosystem-services in Costa Rica.
6. **Limit emergency powers explicitly.** Failure case: Weimar Article 48. Positive cases: Swiss federal emergency provisions with explicit review.
7. **Federate cooperatives and commons rather than depending on single nodes.** Mondragon, Ostrom design principles.
8. **Maintain feedback channels even under stress.** USSR's failure was largely feedback failure; democratic backsliding closes feedback first.

## Caveats and Selection Bias

- Surviving institutions are over-sampled by definition; survivorship bias is structural here.
- Romanticization risk for non-Western and indigenous benchmarks is real; entries should be reviewed by relevant communities before "validated" status.
- Several benchmarks were authoritarian or imperial in significant ways (Singapore, Byzantine, Tokugawa); design lessons extracted here are explicitly partial.
- Future iterations should add more Global South and post-colonial benchmarks, and more failure cases from a broader regional spread.
