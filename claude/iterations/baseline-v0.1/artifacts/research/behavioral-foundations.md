# Behavioral Foundations

Artifact ID: ART-007
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: MOD-RES
Depends on: ART-003, ART-004

## Purpose

Document the behavioral assumptions the framework relies on, with explicit evidence strength and scope conditions. The goal is to design institutions that work with realistic humans — bounded, emotional, social, partly cooperative, partly self-interested, partly tribal — rather than with the idealized agents of either neoclassical economics or romanticized communitarianism.

This artifact is descriptive (what we believe humans tend to do under specified conditions). Normative claims about how humans *should* be treated live in `value-constitution.md` (ART-008).

## Core Behavioral Profile

Humans, on average and under most conditions, exhibit the following properties. Each property is tagged with the relevant claim from `evidence-matrix.md` and the institutional implication.

### B-001 Bounded rationality

People reason with limited attention, memory, and computation; rely heavily on heuristics; and are systematically biased in well-documented ways.

- Evidence: large psychology and behavioral-economics literature; classical findings on availability, anchoring, framing, loss aversion remain replicated despite reproducibility debates on specific effects.
- Confidence: High for the general claim; Medium for the magnitude of any specific bias.
- Institutional implication: rules and choice architectures matter; defaults should be set with care; one-shot consent regimes are insufficient for high-stakes decisions; institutions should rehearse decisions before crisis, not improvise.

### B-002 Social motivation runs deep

People care about social standing, group belonging, and perceived fairness even at material cost to themselves. Status, dignity, and shame are first-order motivators.

- Evidence: CLM-040, CLM-090; ultimatum-game evidence, status-syndrome research, procedural-justice literature.
- Confidence: High.
- Institutional implication: design must take dignity and procedural fairness seriously; ignoring them produces compliance failure and legitimacy loss; status hierarchies are inevitable but their content and steepness are policy-shapable.

### B-003 Cooperation is conditional and learnable

Most people are conditional cooperators: they will cooperate when they expect others to and when they trust enforcement against defection.

- Evidence: CLM-150, CLM-151; public-goods experiments across cultures.
- Confidence: High.
- Institutional implication: visibility of others' cooperation matters; weak enforcement against egregious defection collapses cooperation; small group of unconditional defectors can degrade outcomes without enforcement.

### B-004 Trust is built locally and generalizable with effort

Most humans trust kin and immediate community more than strangers. Generalized trust toward strangers is supported by stable institutions, norms of impersonal exchange, and education.

- Evidence: CLM-150, CLM-160; cross-cultural trust experiments (SRC-090, SRC-092).
- Confidence: Medium-High; cultural variation is significant.
- Institutional implication: institutions must build legibility of strangers (identity, contract, conflict-resolution) and protect against fraud, or generalized trust will recede toward kin networks.

### B-005 Tribal in-group / out-group dynamics are strong and modulable

Identity-based group boundaries activate quickly and predict behavior. Minimal-group experiments show even arbitrary group assignment changes behavior. Cross-cutting identities and superordinate goals moderate in-group bias.

- Evidence: classical minimal-group studies; intergroup-contact literature; ethnic conflict scholarship.
- Confidence: Medium-High.
- Institutional implication: design must avoid amplifying single-axis identity cleavages and should create cross-cutting institutions, shared infrastructure, and superordinate civic identity.

### B-006 Strong reciprocity, including costly punishment

Many humans punish norm violators even at personal cost. Strong reciprocators support cooperative equilibria; absence of enforcement collapses them.

- Evidence: lab and field experiments on costly punishment (SRC-057, SRC-090).
- Confidence: High.
- Institutional implication: legitimate, fair enforcement is a behavioral, not just regulatory, requirement; private-vendetta punishment is destructive; formal institutions must channel reciprocity into legitimate sanction.

### B-007 Group size shapes governance form

Cognitive constraints on stable interpersonal relationships and reputation tracking place limits on which governance forms are workable at which scale. Direct mutual-monitoring relations work for small groups; larger groups require formal mechanisms.

- Evidence: CLM-062 (Dunbar layering); ethnographic and social-network research.
- Confidence: Medium.
- Institutional implication: governance design should be multi-scale; small groups can use informal mechanisms but larger groups need formal procedures, identity systems, and accountability infrastructure.

### B-008 Attachment shapes lifespan capacity

Early attachment quality and adversity shape stress regulation, social functioning, and physical health across the lifespan.

- Evidence: CLM-043, CLM-063 (ACEs, Bowlby and successors).
- Confidence: High.
- Institutional implication: family supports, early childhood services, trauma-informed institutions are foundational, not optional; trauma exposure compounds across generations without intervention.

### B-009 Trauma changes behavior at scale

Population-level trauma (war, displacement, abuse, neglect, poverty stress) shifts behavioral baselines: reduced trust, increased threat-detection, lower long-term planning, worse health.

- Evidence: ACEs literature; collective-trauma research; refugee mental-health studies.
- Confidence: High.
- Institutional implication: post-conflict and post-disaster contexts require trauma-informed institutional default; framework design must include trauma recovery as a normal institutional function.

### B-010 Loss aversion and status quo bias

Losses weigh more than equivalent gains; people resist change even when it would benefit them, especially in uncertain conditions.

- Evidence: prospect theory; behavioral-economics replications.
- Confidence: High.
- Institutional implication: transitions must address loss explicitly; just-transition compensation matters; insurance and guarantees reduce reform resistance.

### B-011 Time discounting is steep but contextual

Most people heavily weight near-term outcomes; future-self is treated almost like a stranger. Time discounting can be moderated by framing, commitment devices, and social context.

- Evidence: standard behavioral findings; commitment-device experiments.
- Confidence: High for short-term bias; Medium for malleability magnitude.
- Institutional implication: future-oriented decisions need institutional support (commitment devices, future-generations advocates, long-horizon decision rules); democratic majoritarianism alone tends to under-invest in the future.

### B-012 Motivation is multidimensional

Autonomy, competence, and relatedness needs predict intrinsic motivation, wellbeing, and durable engagement. External rewards can crowd out intrinsic motivation in some contexts.

- Evidence: CLM-051 (Self-Determination Theory); replicated cross-culturally.
- Confidence: High.
- Institutional implication: work, school, civic participation, healthcare, and care relationships should preserve autonomy, support competence, and enable relatedness; pure extrinsic reward systems erode motivation over time.

### B-013 Capacity for change exists but is bounded

Adults can change beliefs, skills, and behaviors with effort and support, but personality traits, deep beliefs, and addictions show high stability.

- Evidence: longitudinal personality research; learning-science meta-analyses; addiction research.
- Confidence: High.
- Institutional implication: education and reintegration systems are realistic but should not assume infinite plasticity; addiction and severe mental illness require sustained structural support.

### B-014 Group cognition can outperform individuals

Diverse groups with structured deliberation often outperform individuals on complex problems. Same groups under bad procedure (anchoring, dominance, polarization) underperform.

- Evidence: SRC-013, SRC-089; deliberative-poll evidence; jury research.
- Confidence: Medium-High.
- Institutional implication: deliberation requires procedure and facilitation; ad hoc majority voting in small groups can produce worse results than structured deliberation.

### B-015 Information environment shapes belief formation

Beliefs about social reality (others' opinions, fairness norms, threat levels) are strongly influenced by perceived information environment. Algorithmic recommender systems can shift those perceptions at scale.

- Evidence: media-effects literature; recent recommender-system research.
- Confidence: Medium-High.
- Institutional implication: information infrastructure is civic infrastructure; oversight of high-reach systems is part of civic governance.

### B-016 Stress, scarcity, and cognitive bandwidth

Material scarcity, chronic stress, and acute fear reduce executive function, planning horizon, and prosocial behavior.

- Evidence: scarcity-and-bandwidth research; stress-physiology literature.
- Confidence: High.
- Institutional implication: relieving material insecurity is a precondition for high-functioning citizenship; demanding civic capacity from chronically stressed populations is unfair and ineffective.

### B-017 Adversarial environments and learned helplessness

Repeated experience of injustice, capricious authority, or futility predicts disengagement, distrust, and reduced future-orientation across generations.

- Evidence: learned-helplessness literature; political-disengagement research.
- Confidence: Medium-High.
- Institutional implication: visibly responsive institutions are themselves a behavioral intervention; non-responsive institutions produce structural disengagement.

### B-018 Identity is multiple and context-cued

People hold multiple identities (family, ethnic, regional, professional, religious, civic, ideological). Context cues which identity is salient. Designed contexts can elicit cooperative or competitive identities.

- Evidence: self-categorization theory; cross-cultural identity research.
- Confidence: Medium-High.
- Institutional implication: civic identity can be built without erasing other identities; rituals, shared infrastructure, and superordinate goals can elicit it.

### B-019 Norms are sticky but can shift

Social norms are stable until tipping points; once tipped, they can shift rapidly (smoking, drunk driving, same-sex marriage attitudes in many countries).

- Evidence: norm-cascade research.
- Confidence: Medium-High.
- Institutional implication: long-horizon norm change is possible with sustained signaling and institutional reinforcement; norm campaigns alone without structural change usually fail.

### B-020 Capacity for moral injury and meaning collapse

People can be psychologically damaged by participation in or witness to deep moral violations, including by their own institutions.

- Evidence: moral-injury literature, particularly in veterans, healthcare workers, refugees.
- Confidence: Medium-High.
- Institutional implication: institutions that require staff to act against deep moral commitments degrade those staff over time and lose function; ethical fitness is a maintenance concern, not a hiring concern only.

## Scope Conditions and Cultural Variation

Most of the above is supported primarily by research conducted in WEIRD populations (CLM-060). The framework treats these findings as default tendencies but expects:

- Magnitudes and even directions of some effects vary cross-culturally.
- Local research and participatory design are required before adapting any specific institutional design across cultural contexts.
- Indigenous, religious, and traditional communities may have governance and cooperation forms that operate on different mechanisms than those documented in the WEIRD literature; these are valuable references, not deviations.

## Design Heuristics Derived from Behavior

From the above, several institutional design heuristics follow:

1. **Make cooperation visible, defection detectable, and enforcement legitimate.** (B-003, B-006)
2. **Treat dignity and procedural fairness as enforcement-grade requirements.** (B-002)
3. **Build cross-cutting civic identity without erasing prior identities.** (B-005, B-018)
4. **Design institutions for trauma-informed default operation.** (B-008, B-009)
5. **Use commitment devices and future-advocate institutions to overcome short-termism.** (B-011)
6. **Preserve autonomy, competence, and relatedness in work, school, and civic life.** (B-012)
7. **Relieve material scarcity to enable functional citizenship.** (B-016)
8. **Build information infrastructure as civic infrastructure.** (B-015)
9. **Provide structured deliberation, not raw voting, on complex contested issues.** (B-014)
10. **Make institutions visibly responsive to weak signals before they become crises.** (B-017; mitigates RSK-043)
11. **Plan for norm shifts on multi-generational horizons.** (B-019)
12. **Limit the personal moral cost of working in public institutions.** (B-020)

## Open Issues

- The interaction of digital-environment effects (B-015) with intrinsic-motivation findings (B-012) under recommender systems is poorly characterized; specific design choices in MOD-TAI must be tested rather than assumed.
- The trauma literature relies heavily on selected samples; quantitative effect sizes should be treated cautiously when designing benefits.
- The framework currently under-specifies how to operate amid populations with very high prior-trauma loads; module updates should address this with case-specific evidence.
- We rely on the assumption that institutional environment can shift behavior over generational timescales (B-019). If it cannot in the relevant window, several mitigations in `failure-mode-register.md` weaken.
