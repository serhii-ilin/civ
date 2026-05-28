# Evidence Matrix

Artifact ID: ART-004
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: MOD-RES
Depends on: ART-003

## Purpose

Master claim catalog. Every claim used to justify a design decision in this iteration is registered here with classification (`[ESTABLISHED]`, `[CONTESTED]`, `[THEORETICAL]`, `[ASSUMPTION]`, `[NORMATIVE]`), supporting sources from `source-register.md`, confidence rating, and the artifact(s) that consume the claim.

Claims are grouped by topic. Boundary conditions and known counter-evidence are recorded in the `Notes` field of each row when relevant; full discussion of contested claims lives in `contradiction-register.md` (ART-029) when the contradiction affects the framework.

## Confidence Scale

- High: replicated meta-analyses or convergent multi-method evidence; would require strong new evidence to overturn.
- Medium: supported by reasonable evidence but with notable caveats, scope conditions, or moderate replication.
- Low: limited evidence, contested, or strongly model-dependent; treat as provisional.

## Claim Table

### History and institutional collapse (CLM-001 to CLM-031)

| Claim ID | Claim | Classification | Source IDs | Confidence | Used In | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| CLM-001 | Complex societies face declining marginal returns on additional layers of administrative complexity. | [CONTESTED] | SRC-001 | Medium | ART-006, ART-009, ART-018 | Tainter's frame is one explanation among several; useful as design caution. |
| CLM-002 | Civilizations have failed through combinations of ecological overshoot, internal political fragmentation, external shock, and elite mismanagement, rarely from a single cause. | [ESTABLISHED] | SRC-001, SRC-002, SRC-064, SRC-073 | High | ART-006 | Selection bias in Diamond (SRC-073) is noted; do not rely on him alone. |
| CLM-003 | Inclusive political and economic institutions correlate with long-run growth and resilience compared to extractive institutions, controlling for geography. | [CONTESTED] | SRC-002, SRC-003 | Medium | ART-009, ART-010 | Inclusive/extractive distinction can be circular; treat directionally. |
| CLM-004 | Concentration of property rights and political access in a narrow elite tends to entrench across generations absent strong countervailing institutions. | [ESTABLISHED] | SRC-002, SRC-014, SRC-070 | High | ART-009, ART-010 | Strong cross-country and within-country evidence. |
| CLM-005 | Liberty-conducive equilibria are unstable without continual balancing between state capacity and civil society. | [THEORETICAL] | SRC-003 | Medium | ART-009 | Theoretical framework with selected historical illustrations. |
| CLM-006 | Major reductions in inequality in modern history have followed mass-mobilization war, revolution, state collapse, or pandemic. | [CONTESTED] | SRC-004 | Medium | ART-010 | Scheidel's thesis ignores some peaceful redistribution episodes; treat as warning, not law. |
| CLM-007 | Societal stress cycles correlate with elite overproduction, inequality, and declining state legitimacy. | [CONTESTED] | SRC-005, SRC-063 | Medium | ART-009, ART-010, ART-014 | Cliodynamic mechanisms not all causally identified. |
| CLM-010 | Long-lived commons regimes share design features: clear boundaries, congruence between rules and local conditions, collective-choice arenas, monitoring, graduated sanctions, conflict-resolution access, recognition by external authority, and nested governance. | [ESTABLISHED] | SRC-006 | High | ART-010, ART-014, ART-015 | Ostrom's eight design principles; widely replicated across commons types. |
| CLM-011 | Indigenous and small-scale resource governance has, in many documented cases, sustained ecosystems across centuries. | [ESTABLISHED] | SRC-006, SRC-075 | High | ART-014, ART-015 | Generalization to large industrial systems requires careful translation. |
| CLM-012 | Dense civic associational life predicts higher institutional performance, trust, and adaptive capacity in many contexts. | [CONTESTED] | SRC-007, SRC-008 | Medium | ART-014, ART-009 | Causal direction contested; pair with intervention evidence. |
| CLM-013 | Civic culture and institutional performance co-evolve, but path-dependence makes rapid imitation across regions difficult. | [CONTESTED] | SRC-008 | Medium | ART-018, ART-024 | Putnam's Italian study; northern-southern Italy interpretation contested. |
| CLM-014 | Durable state capacity rests on three pillars: state capacity proper, rule of law, and accountability to non-state actors. | [THEORETICAL] | SRC-009, SRC-010 | Medium | ART-009 | Synthetic framework; supported by selected cases. |
| CLM-015 | Modern democracies decay primarily through gradual erosion of norms and informal constraints, not single coups. | [ESTABLISHED] | SRC-011, SRC-051 | High | ART-009, ART-011, ART-017 | Pattern-matched across many recent cases. |
| CLM-016 | Aspiring autocrats consolidate power by capturing courts, electoral administration, security services, and media before contesting formal rules. | [ESTABLISHED] | SRC-011 | High | ART-009, ART-011 | Convergent across cases. |
| CLM-017 | Election-based representation introduces aristocratic features (selection for prominence and wealth) that pure democratic theory does not justify. | [THEORETICAL] | SRC-012 | Medium | ART-009 | Manin's argument; pair with empirical work on candidate selection. |
| CLM-018 | Randomly selected citizen bodies (sortition) can deliberate effectively on complex policy when given sufficient time and facilitation. | [CONTESTED] | SRC-013, SRC-088, SRC-089 | Medium | ART-009 | Many small-scale demonstrations; durability at scale untested. |
| CLM-020 | Wealth concentrations near the top decile and percentile in advanced economies have grown substantially since the late twentieth century. | [ESTABLISHED] | SRC-014, SRC-015, SRC-070 | High | ART-010 | Multi-source convergence; methodology details disputed at margins. |
| CLM-021 | The top 1 percent's income share varies considerably across high-income countries with similar productivity, indicating that policy and institutions, not productivity alone, drive inequality outcomes. | [ESTABLISHED] | SRC-015, SRC-020 | High | ART-010 | Comparative WID data. |
| CLM-022 | Effective tax rates on top earners in the United States have declined since mid-twentieth century, particularly through capital income channels. | [CONTESTED] | SRC-016 | Medium | ART-010 | Methodology disputed by alternative public-finance estimates. |
| CLM-023 | Many foundational technologies in advanced economies trace early funding to mission-oriented public investment. | [CONTESTED] | SRC-017 | Medium | ART-010, ART-016 | Case-study evidence; counterfactual claims weaker than headline narrative. |
| CLM-024 | Designing economies for inner social floors and outer ecological ceilings is intellectually coherent and operationalizable through composite indicators. | [THEORETICAL] | SRC-018 | Medium | ART-010, ART-015 | Framework, not validated outcome model. |
| CLM-025 | Randomized field evidence finds many anti-poverty interventions produce durable effects only when bundled with complementary supports. | [ESTABLISHED] | SRC-019 | High | ART-010, ART-012, ART-013 | RCT-based; scope conditions documented in primary papers. |
| CLM-026 | Welfare-state typologies (residual, conservative, social-democratic) shape labor-market behavior, fertility, family stability, and inequality. | [CONTESTED] | SRC-020, SRC-087, SRC-102 | Medium | ART-010, ART-012 | Typology contested; broad correlations robust. |
| CLM-027 | Standard GDP-maximizing growth and ecological-limit compliance cannot both be optimized indefinitely on a finite planet under current resource and energy intensities. | [ESTABLISHED] | SRC-021, SRC-036, SRC-037, SRC-038 | High | ART-010, ART-015 | Decoupling at sufficient speed is unproven; treat as design constraint. |
| CLM-028 | Robotization in the United States has produced negative local labor-market effects on employment and wages, with heterogeneity across industries and regions. | [CONTESTED] | SRC-022 | Medium | ART-010, ART-016 | Industry-level identification; magnitudes debated. |
| CLM-030 | Bureaucratic over-elaboration without functional gain is a recurring late-stage feature of declining polities. | [CONTESTED] | SRC-001 | Medium | ART-009 | Pattern-claim; difficult to operationalize. |
| CLM-031 | Demographic-structural pressure (youth bulges, elite over-production, fiscal strain) predicts elevated risk of political instability with significant lead time. | [CONTESTED] | SRC-005, SRC-063 | Medium | ART-009, ART-014 | Mechanism-rich; calibration debated. |

### Health, mental health, and social determinants (CLM-040 to CLM-053)

| Claim ID | Claim | Classification | Source IDs | Confidence | Used In | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| CLM-040 | Position in social and economic hierarchies independently predicts physical health outcomes after accounting for absolute material conditions. | [ESTABLISHED] | SRC-023, SRC-024 | High | ART-010, ART-012 | Whitehall and replications. |
| CLM-041 | More equal societies show better aggregate health and social outcomes than less equal ones at comparable income levels. | [CONTESTED] | SRC-025 | Medium | ART-010, ART-012 | Correlational; causal pathways contested. |
| CLM-042 | Social isolation and loneliness increase all-cause mortality risk at magnitudes comparable to major behavioral risk factors. | [ESTABLISHED] | SRC-026, SRC-084 | High | ART-012, ART-014 | Robust meta-analytic finding. |
| CLM-043 | Adverse childhood experiences (ACEs) correlate dose-dependently with adult physical and mental health problems. | [ESTABLISHED] | SRC-027 | High | ART-012, ART-013, ART-014 | Replicated; recall and selection caveats noted in primary work. |
| CLM-050 | Teacher quality and instructional clarity are among the larger school-side effects on learning outcomes; effect sizes are smaller than out-of-school determinants. | [ESTABLISHED] | SRC-028, SRC-030 | High | ART-013 | Meta-meta-analysis; effect-size method critiques accepted. |
| CLM-051 | Intrinsic motivation supports durable learning and wellbeing more reliably than external rewards alone. | [ESTABLISHED] | SRC-029 | High | ART-013, ART-014 | Cross-cultural replication. |
| CLM-052 | Early childhood investment in disadvantaged children produces high social returns relative to later remediation. | [ESTABLISHED] | SRC-030 | High | ART-013, ART-024 | Specific program evidence; generalization caveats noted. |
| CLM-053 | School systems with strong support for teachers, equitable resource allocation, and moderate accountability outperform those built primarily on standardized-test pressure on measured learning. | [CONTESTED] | SRC-031 | Medium | ART-013 | PISA-based; system-design causal claims debated. |

### Behavioral and cultural science (CLM-060 to CLM-063)

| Claim ID | Claim | Classification | Source IDs | Confidence | Used In | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| CLM-060 | Western, Educated, Industrialized, Rich, Democratic (WEIRD) populations are not representative of human cognitive and behavioral variation. | [ESTABLISHED] | SRC-032, SRC-066 | High | ART-013, ART-014, ART-007 | Methodological caution for any psychometric claim. |
| CLM-061 | Cultural transmission, not only individual cognition, accounts for much of humanity's adaptive capacity. | [ESTABLISHED] | SRC-033 | High | ART-007, ART-014 | Convergent evidence across anthropology and experimental psychology. |
| CLM-062 | Cognitive limits on stable interpersonal relationships likely fall in a low-hundreds order of magnitude, with social-network layering above that. | [CONTESTED] | SRC-034 | Medium | ART-014 | "Dunbar's number" is an estimate band, not a hard threshold. |
| CLM-063 | Early-life attachment quality shapes regulation, social functioning, and stress response across the lifespan. | [ESTABLISHED] | SRC-035 | High | ART-012, ART-013, ART-014 | Bowlby foundations updated by later attachment research. |

### Ecology and planetary boundaries (CLM-070 to CLM-075)

| Claim ID | Claim | Classification | Source IDs | Confidence | Used In | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| CLM-070 | A bounded set of Earth-system processes plausibly defines a safe operating space for humanity. | [THEORETICAL] | SRC-036 | Medium | ART-015 | Framework; specific boundary values revised periodically. |
| CLM-071 | At present, multiple planetary boundaries are estimated to be transgressed simultaneously. | [CONTESTED] | SRC-037 | Medium | ART-015 | Methodological evolution continues; treat as warning, not point estimate. |
| CLM-072 | Continued greenhouse gas emissions will produce severe and unevenly distributed climate impacts, with risks rising non-linearly past 1.5 to 2 degrees Celsius warming. | [ESTABLISHED] | SRC-038 | High | ART-015, ART-017 | IPCC consensus. |
| CLM-073 | Global biodiversity loss is occurring at rates far above background extinction levels. | [ESTABLISHED] | SRC-039 | High | ART-015 | IPBES assessment. |
| CLM-074 | Food systems are simultaneously a major contributor to ecological pressure and dependent on ecological stability. | [ESTABLISHED] | SRC-040, SRC-039 | High | ART-015, ART-010 | Cross-sectoral evidence. |
| CLM-075 | Energy transitions historically take decades and require mineral, capital, labor, and grid build-out, even with strong policy. | [ESTABLISHED] | SRC-041 | High | ART-015, ART-024 | IEA scenarios; conservative on disruption. |

### Commons, surveillance, and technology (CLM-080 to CLM-085)

| Claim ID | Claim | Classification | Source IDs | Confidence | Used In | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| CLM-080 | Commercial behavioral-data extraction has scaled into a structural feature of digital economies. | [CONTESTED] | SRC-042 | Medium | ART-016 | Zuboff's framing critiqued; underlying data-market evidence is robust. |
| CLM-081 | Predictive algorithms deployed in high-stakes settings can reproduce and amplify historical patterns of disadvantage when trained on historical outcomes. | [ESTABLISHED] | SRC-043, SRC-044, SRC-045 | High | ART-016, ART-011 | Convergent technical and audit evidence. |
| CLM-082 | Public-sector algorithmic systems applied to welfare, child protection, and policing have, in documented cases, produced procedurally unfair and inaccurate outcomes. | [ESTABLISHED] | SRC-044 | High | ART-011, ART-016 | Ethnographic and audit evidence. |
| CLM-083 | Mandatory algorithmic audit, documentation, and tiered risk regulation are technically feasible for many AI applications. | [THEORETICAL] | SRC-045, SRC-079 | Medium | ART-016 | Regulatory frameworks new; long-run effectiveness unproven. |
| CLM-084 | Specifying robust objectives for capable AI systems, in domains with rich preference structures, remains an unsolved research problem. | [THEORETICAL] | SRC-046 | Medium | ART-016 | Active research area; treat as live design constraint. |
| CLM-085 | Critical-infrastructure cyber risk is concentrated in a small set of sectors with interdependencies; cascading failure across them is plausible. | [ESTABLISHED] | SRC-077, SRC-078 | High | ART-016, ART-017 | NIST/CISA taxonomies and incident data. |

### Procedural justice and law (CLM-090 to CLM-091, CLM-189 to CLM-193)

| Claim ID | Claim | Classification | Source IDs | Confidence | Used In | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| CLM-090 | Perceived procedural fairness of authorities predicts compliance, cooperation, and legitimacy independently of outcome favorability. | [ESTABLISHED] | SRC-047 | High | ART-009, ART-011, ART-014 | Widely replicated. |
| CLM-091 | Restorative-justice programs reduce repeat offending in selected offence types and victim populations more than retribution-focused responses, with high variance by program design. | [CONTESTED] | SRC-048, SRC-049, SRC-101 | Medium | ART-011 | Evidence quality varies; effective design features are partly known. |
| CLM-189 | Targeting a measured indicator tends to distort the indicator and the underlying behavior it was meant to track (Goodhart, Campbell). | [ESTABLISHED] | SRC-071, SRC-072 | High | ART-009, ART-010, ART-018, ART-019 | Foundational design caution. |
| CLM-190 | International human-rights instruments enumerate a stable core of civil, political, economic, social, and cultural rights that have been adopted into most national constitutions. | [ESTABLISHED] | SRC-080 | High | ART-008, ART-011 | Adoption does not equal implementation; pair with enforcement evidence. |
| CLM-191 | Discrimination on the basis of name, race, gender, and other markers is detectable in audit experiments across labor, housing, and credit markets in multiple countries. | [ESTABLISHED] | SRC-069 | High | ART-011, ART-014 | Convergent audit evidence. |
| CLM-192 | Effective policing depends more on consistent, lawful, low-coercion engagement than on aggregate force levels. | [CONTESTED] | SRC-082 | Medium | ART-011 | Jurisdiction-specific; mechanism well documented. |
| CLM-193 | Neighborhood-level collective efficacy predicts safety outcomes after controlling for poverty and demographics. | [ESTABLISHED] | SRC-083 | Medium | ART-014 | Robust within studied contexts; generalization debated. |

### Inequality, mobility, and wellbeing (CLM-100 to CLM-132)

| Claim ID | Claim | Classification | Source IDs | Confidence | Used In | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| CLM-100 | Democratic backsliding accelerated across multiple regions in the 2010s and 2020s, measured by independent expert indices. | [ESTABLISHED] | SRC-011, SRC-051, SRC-052, SRC-096 | High | ART-009, ART-017 | Multi-source convergence; measurement caveats acknowledged. |
| CLM-101 | Constitutional design choices (federalism, judicial review, electoral system, executive type) measurably shape long-run political stability and rights outcomes. | [ESTABLISHED] | SRC-012, SRC-051, SRC-081, SRC-093 | High | ART-009 | Magnitudes contested; presence of effect is robust. |
| CLM-102 | Public participation through deliberative methods can improve perceived legitimacy and policy quality on selected questions. | [CONTESTED] | SRC-013, SRC-089 | Medium | ART-009 | Durability and scaling unproven. |
| CLM-110 | Inter-generational economic mobility varies substantially across countries and within countries, and is strongly shaped by neighborhood, school, and family conditions. | [ESTABLISHED] | SRC-014, SRC-015, SRC-070, SRC-086 | High | ART-010, ART-013 | US data is most granular; cross-country evidence robust. |
| CLM-111 | Pre-tax inequality and post-tax-transfer inequality diverge significantly across welfare regimes with similar productivity. | [ESTABLISHED] | SRC-015, SRC-087 | High | ART-010 | Policy-driven divergence. |
| CLM-120 | Composite human-capability indicators (HDI, capability approaches) capture welfare information that GDP alone does not. | [ESTABLISHED] | SRC-018, SRC-095, SRC-097, SRC-098 | High | ART-010, ART-018 | Composite limits flagged in primary sources. |
| CLM-130 | Subjective wellbeing is reliably measurable within cultures and correlates with social trust, health, employment, and freedom, with weaker cross-cultural comparability. | [ESTABLISHED] | SRC-054, SRC-076, SRC-099 | Medium | ART-012, ART-014 | Measurement caveats well documented. |
| CLM-131 | Mental health conditions account for a substantial share of total global disease burden, with large treatment gaps. | [ESTABLISHED] | SRC-055, SRC-067 | High | ART-012 | Global burden of disease estimates. |
| CLM-132 | Community-based and task-shifted mental-health interventions are cost-effective in low- and middle-resource contexts. | [ESTABLISHED] | SRC-067, SRC-068 | High | ART-012, ART-024 | Lancet Commission evidence. |

### Behavioral foundations and cooperation (CLM-150 to CLM-153)

| Claim ID | Claim | Classification | Source IDs | Confidence | Used In | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| CLM-150 | Cooperation in repeated interactions is sustained by reciprocity, reputation, and group-level enforcement, with mechanism mix varying by context. | [ESTABLISHED] | SRC-056, SRC-057, SRC-090 | High | ART-007, ART-009, ART-014 | Multiple convergent traditions (game theory, behavioral econ, sociology). |
| CLM-151 | Tit-for-tat and similar simple reciprocal strategies perform well in iterated prisoner's-dilemma tournaments under broad conditions. | [ESTABLISHED] | SRC-057 | High | ART-007, ART-014 | Axelrod's result; well-replicated. |
| CLM-152 | Agent-based models can generate emergent social phenomena (segregation, inequality, cooperation patterns) from simple local rules. | [ESTABLISHED] | SRC-058 | High | ART-019 | Demonstrative; not directly predictive. |
| CLM-153 | Agent-based modeling is appropriate where heterogeneity, local interaction, and adaptation matter; system-dynamics tools fit aggregate flow problems. | [ESTABLISHED] | SRC-059 | High | ART-019 | Methodological guidance. |

### Cross-cutting cultural and historical (CLM-160 to CLM-171)

| Claim ID | Claim | Classification | Source IDs | Confidence | Used In | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| CLM-160 | The expansion of impersonal market relations and prosocial behavior toward strangers correlates historically with specific cultural transmission patterns. | [CONTESTED] | SRC-032, SRC-065, SRC-066 | Medium | ART-014 | SRC-065 specifically has been disputed in re-analyses. |
| CLM-170 | Twentieth-century industrialization produced unprecedented absolute changes in resource use, pollution, and biological systems. | [ESTABLISHED] | SRC-064, SRC-074 | High | ART-015 | Environmental history consensus. |
| CLM-171 | Climate change increases the frequency and severity of selected extreme weather events with measurable economic impact. | [ESTABLISHED] | SRC-038 | High | ART-015, ART-024 | IPCC consensus; attribution science matured. |

### Defense, external relations, and IR (CLM-200 to CLM-201)

| Claim ID | Claim | Classification | Source IDs | Confidence | Used In | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| CLM-200 | Anarchic international systems produce systemic security dilemmas that can drive even defensively oriented states into competitive military posture. | [THEORETICAL] | SRC-061 | Medium | ART-017 | Realist framework; explicitly theoretical. |
| CLM-201 | States balance against threats more than power, weighing geographic proximity, offensive capability, and perceived intent. | [CONTESTED] | SRC-062 | Medium | ART-017 | Walt's balance-of-threat; supported by selected case studies. |

## Coverage Notes

- Modules MOD-CUL, MOD-EDU, and MOD-DEF have lighter empirical coverage in this baseline; future iterations should expand source breadth.
- Most behavioral evidence is WEIRD-biased (see CLM-060). Treat psychometric claims as conditional on context.
- Geographic coverage of governance and welfare claims skews toward OECD countries; targeted iterations should add Global South sources.

## Open Issues

- CLM-022 vs. alternative tax-incidence methodologies: not adjudicated here. Pending review by a future iteration with public-finance focus.
- CLM-006 (Scheidel) is retained as a design caution rather than a binding finding; the framework's redistribution mechanisms should not rely on it.
- CLM-018 sortition durability at scale is an open empirical question; design choice in ART-009 must address this with hedges.
