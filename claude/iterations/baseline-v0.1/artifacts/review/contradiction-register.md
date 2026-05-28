# Contradiction Register

Artifact ID: ART-029
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: all

## Purpose

Record internal contradictions in the framework: tensions between two or more design choices, values, or assumptions that cannot be resolved by appeal to a higher principle and must therefore be managed institutionally.

Per `evidence-standard.md`, contradictions are explained, not silently resolved. The register identifies each, names the affected modules and values, describes the tension concretely, and either records the resolution (with explicit cost-bearing) or leaves the contradiction open with a path for further work.

## Format

```text
CON-XXX | Affected Modules / Values | Description | Resolution Options | Resolution Choice | Cost Borne By | Status
```

## Contradictions

### CON-001 | Liberty vs. Security under crisis

- Affected: VAL-001, VAL-004, VAL-019; ART-009 GOV-D5; ART-011 LAW-E; ART-017 DEF-C.
- Description: emergency powers necessary to address severe shocks restrict rights; over-restriction causes lasting damage; under-restriction risks shock outcomes.
- Resolution options: (a) shorter sunsets and tighter judicial review; (b) explicit risk-tier authorization with different threshold; (c) categorical non-derogable list.
- Resolution choice: explicit non-derogable list (LAW-R5) plus short sunsets (GOV-D5 default 30 days, max cumulative 180 days without supermajority) plus continuing judicial review.
- Cost borne by: short-term efficacy of crisis response in some scenarios; framework accepts this for rights protection.
- Status: Resolved with documented tradeoff (TZ-001); revisit if scenarios show repeated failure of crisis response.

### CON-002 | Pluralism vs. Anti-pluralism

- Affected: VAL-010, VAL-001, VAL-008.
- Description: an anti-pluralist movement that uses constitutional protections to pursue elimination of pluralism poses a paradox.
- Resolution options: (a) suppress anti-pluralist speech / association; (b) protect speech, regulate only specific harms.
- Resolution choice: protect belief and speech under VAL-010; regulate conduct that violates others' rights under VAL-008 (TZ-002); distinguish belief (protected) from conduct (regulated).
- Cost borne by: those who would prefer faster suppression of harmful movements.
- Status: Resolved with documented tradeoff (TZ-002); revisit if speech protection produces movement-led rights erosion before law-based response.

### CON-003 | Self-correction vs. Stability

- Affected: VAL-018, VAL-004; ART-008 Article V; ART-009 GOV-D2.
- Description: too easy amendment produces instability; too hard produces sclerosis.
- Resolution options: (a) low thresholds and frequent review; (b) high thresholds with rare amendments; (c) tiered thresholds by impact.
- Resolution choice: tiered thresholds by impact (operational rules low; constitutional rules high with public deliberation period); periodic constitutional review every 20-25 years (TZ-003).
- Cost borne by: those who would prefer faster or slower amendment.
- Status: Resolved with tradeoff (TZ-003).

### CON-004 | Transparency vs. Privacy

- Affected: VAL-019, VAL-015; ART-016 TAI-O, TAI-D.
- Description: maximal transparency on institutions risks revealing personal information; maximal privacy on individuals risks shielding institutional actors and decisions.
- Resolution options: (a) institutions public, individuals private with default to publish; (b) institutions private, individuals public; (c) institutions public by default but with redaction.
- Resolution choice: institutions observable, individuals private; aggregation and redaction for personal data; cryptographic separation (DEC-020).
- Cost borne by: completeness of public reporting in cases involving named individuals.
- Status: Resolved with documented tradeoff (TZ-004).

### CON-005 | Competence vs. Democratic Legitimacy

- Affected: VAL-005, VAL-007; ART-009 GOV-S3, GOV-S2, GOV-S1.
- Description: technical decisions can require competence not produced by election; full technocracy lacks legitimacy.
- Resolution options: (a) competence-gating across most roles; (b) electoral selection for most roles; (c) hybrid by role.
- Resolution choice: hybrid by role; competence-gating for technical roles (judges, central bankers, regulators, certain executive functions); democratic selection for direction-setting; sortition for value-contested questions (TZ-005).
- Cost borne by: simplicity; system is more complex than a single selection method.
- Status: Resolved with documented tradeoff (TZ-005).

### CON-006 | Local autonomy vs. Universal rights

- Affected: VAL-001, VAL-010; ART-014 CUL-P, ART-018 TAR-P1.
- Description: subsidiarity supports local autonomy; universal rights bind locally.
- Resolution options: (a) full local autonomy; (b) full universal-rights primacy; (c) presumption of local with rights ceiling.
- Resolution choice: presumption of local with universal rights as ceiling enforced by national courts (TZ-006).
- Cost borne by: communities that wished to enforce locally restrictive norms inconsistent with universal rights.
- Status: Resolved with documented tradeoff (TZ-006); specific case-by-case interpretation by courts.

### CON-007 | Present wellbeing vs. Future generations

- Affected: VAL-016, VAL-005; ART-009 GOV-B7, ART-015 ECN-B.
- Description: democratic majority of present generation can legitimately decide on present consumption; future generations cannot vote; ecological limits constrain present consumption.
- Resolution options: (a) present-generation majoritarianism; (b) explicit future-generations veto; (c) consultative future-generations representation plus binding ecological caps.
- Resolution choice: consultative future-generations advocate (GOV-B7) plus constitutionally binding ecological caps (ECN-B) (TZ-007); present generation may decide intra-generational tradeoffs but cannot deplete the resource base.
- Cost borne by: present-generation freedom to consume above sustainable rates.
- Status: Resolved with documented tradeoff (TZ-007).

### CON-008 | Universal floor vs. Tax-base sustainability

- Affected: VAL-013, VAL-014; ART-010 ECO-I1, ECO-T.
- Description: universal floor requires substantial revenue; high taxation may trigger capital flight and base erosion.
- Resolution options: (a) reduce floor; (b) reduce tax progressivity; (c) build international cooperation plus exit-friction instruments.
- Resolution choice: build international cooperation and progressive tax mix (wealth, inheritance, land-value, automation) with international engagement; maintain floor; accept revenue risks during transition.
- Cost borne by: floor durability in adverse cooperation environments; need for active international diplomacy.
- Status: Partially resolved; risk tracked in SCN-017 and ASM-019, ASM-020. Open.

### CON-009 | Encryption vs. Investigation

- Affected: VAL-015, VAL-001; ART-016 TAI-S6; ART-011 LAW-P4.
- Description: strong encryption protects rights but constrains some criminal investigations; back-doors expose all users to attack.
- Resolution options: (a) lawful-access back-doors; (b) ban strong encryption; (c) no back-doors, targeted lawful access with judicial process.
- Resolution choice: no back-doors; targeted lawful access; investigative friction accepted.
- Cost borne by: some investigations harder; framework accepts this as price of secure communications for all.
- Status: Resolved with documented tradeoff (DEC-016); revisit if investigative impossibility becomes systemic.

### CON-010 | Restorative justice vs. Victim protection

- Affected: VAL-008, VAL-001; ART-011 LAW-CJ3.
- Description: restorative pathways depend on victim participation; coercive use violates victims, voluntary use leaves cases unresolved.
- Resolution options: (a) victim-veto on restorative path; (b) standard track regardless of victim preference.
- Resolution choice: victim consent required for restorative; alternative formal-track preserved for non-consenting victims.
- Cost borne by: program volume; some cases proceed in formal track that might have benefited from restorative.
- Status: Resolved.

### CON-011 | Pay-ratio cap vs. Firm-formation freedom

- Affected: VAL-014, ECO-MK1, ECO-I2.
- Description: pay-ratio cap may induce fragmentation of firms or relocation; uncapped pay creates inequality dynamics.
- Resolution options: (a) no cap; (b) cap with anti-fragmentation rules; (c) sectoral caps without firm-level caps.
- Resolution choice: firm-level cap with anti-fragmentation rules; sectoral wage boards in addition.
- Cost borne by: administrative complexity; some firms with legitimate need for high disparity find workarounds; framework accepts these costs for structural inequality moderation.
- Status: Resolved with risk tracked in ASM-003 and SCN-017.

### CON-012 | Open immigration vs. Reception capacity

- Affected: VAL-001, VAL-004; ART-017 DEF-MIG.
- Description: rights-respecting asylum and immigration is unbounded in principle; reception capacity is bounded.
- Resolution options: (a) hard caps; (b) no caps; (c) processing capacity with humane defaults under stress.
- Resolution choice: rights-respecting process with capacity scaling; international coordination on burden-sharing; no hard caps that violate non-refoulement; humane defaults including alternatives to detention.
- Cost borne by: reception capacity scaling investments; political contention.
- Status: Resolved with risk tracked in SCN-005 (climate cascade scenario).

### CON-013 | Education depth vs. Capability breadth

- Affected: VAL-011; ART-013 EDU-C.
- Description: broad capability curriculum may sacrifice subject depth; deep specialization may sacrifice civic and practical capability.
- Resolution options: (a) prioritize depth; (b) prioritize breadth; (c) combine with pathway-specialization in upper-secondary.
- Resolution choice: common broad curriculum through lower secondary; pathway specialization in upper secondary (DEC-011).
- Cost borne by: subject specialists who prefer earlier tracking.
- Status: Resolved.

### CON-014 | AI productivity vs. Human autonomy

- Affected: VAL-001, VAL-007; ART-016 TAI-R, ART-010 ECO-W.
- Description: AI deployment can improve productivity and access but can erode human autonomy and competence; full automation in high-stakes domains is prohibited (TAI-R2-R3) but assistance is allowed.
- Resolution options: (a) prohibit all AI use; (b) full automation default; (c) risk-tiered with prohibition in high-stakes domains and human accountability.
- Resolution choice: risk-tiered with prohibition in high-stakes domains; human accountability vested (TAI-AC6).
- Cost borne by: productivity gains forgone in prohibited domains; framework accepts cost.
- Status: Resolved with risk tracked in ASM-009, SCN-008.

### CON-015 | Free press vs. Information disorder

- Affected: VAL-018, VAL-019; ART-014 CUL-MI; ART-016 TAI-R4.
- Description: press freedom is fundamental; recommender algorithms and synthetic media at scale amplify information disorder; regulating speech threatens VAL-001.
- Resolution options: (a) regulate speech directly; (b) no platform regulation; (c) algorithmic-amplification regulation and watermarking.
- Resolution choice: protect speech; regulate amplification, watermarking, and platform transparency; narrow harm-test exceptions.
- Cost borne by: some speech effects on public discourse remain; platforms bear compliance cost.
- Status: Resolved with risk tracked in SCN-008.

### CON-016 | Member observability vs. Whistleblower safety

- Affected: VAL-019, VAL-001, VAL-018; ART-008 TZ-009.
- Description: full observability could expose whistleblower identities; full anonymity could shield false accusations.
- Resolution options: (a) full observability; (b) full anonymity; (c) institutional observability with personal-identity protection for whistleblowers.
- Resolution choice: institutional observability of investigations and outcomes; personal-identity protection for whistleblowers; due process for accused.
- Cost borne by: complete-public-record idealization.
- Status: Resolved.

### CON-017 | Capture-resistant qualification vs. Credentialism

- Affected: VAL-007, VAL-006; ART-009 GOV-S3.
- Description: competence assessment is necessary for some roles but credentialism reproduces class advantage (RSK-028); blunt competence assessment can entrench gatekeeping.
- Resolution options: (a) no competence-gating; (b) standard credentials only; (c) multi-method assessment with bias auditing.
- Resolution choice: multi-method assessment (exam, portfolio, peer, mentor) with transparent rubrics and bias audits; recognition of prior learning; multiple paths to qualification.
- Cost borne by: assessment complexity.
- Status: Resolved with risk tracked in ASM-016, SCN-001 inequality variations.

### CON-018 | Universal services vs. Private innovation

- Affected: VAL-013, VAL-014; ART-010 ECO-L, ECO-IN.
- Description: universal services compete with private provision; private innovation might be discouraged in some sectors.
- Resolution options: (a) full public; (b) full private; (c) plural provision in regulated framework with universal floor.
- Resolution choice: universal services for essentials; plural provision in regulated framework; innovation supported through public investment and patent rules.
- Cost borne by: investor returns in essentials; framework accepts this for floor.
- Status: Resolved.

### CON-019 | Sortition durability vs. Sortition power

- Affected: VAL-005, VAL-018; ART-009 GOV-B1, GOV-B6.
- Description: powerful sortition body is more legitimate but more attractive target for capture; weak body is less attractive but less effective.
- Resolution options: (a) consultative-only; (b) full legislative authority; (c) specified-power with adversarial-review protection.
- Resolution choice: specified powers (deliberation, veto on enumerated categories, confirmation roles) with capture protections.
- Cost borne by: deliberative-democracy advocates wanting full authority; technocrats wanting consultative role.
- Status: Resolved; durability tested in SCN-019.

### CON-020 | Indigenous and customary law vs. Universal rights

- Affected: VAL-001, VAL-010; ART-011 LAW-S5.
- Description: respect for indigenous and customary law recognizes pluralism and historical justice; some customary practices may conflict with universal rights.
- Resolution options: (a) full deference to customary law; (b) full constitutional ceiling; (c) participatory accommodation within rights limits.
- Resolution choice: respect within constitutional limits; conflict-resolution through participatory process; ultimate appeal to constitutional courts; indigenous land and self-governance recognized with rights ceiling.
- Cost borne by: communities preferring full autonomy; framework accepts the cost as price of universal rights.
- Status: Resolved; remains contested in specific cases; participatory design required.

### CON-021 | Universal floor and inflation risk

- Affected: VAL-002, VAL-014; ART-010 ECO-I1, ECO-M1.
- Description: universal floor under inflationary pressure can lose real value; indexing risks wage-price dynamics.
- Resolution options: (a) nominal floor; (b) inflation-indexed floor with macroprudential discipline; (c) supply-side response.
- Resolution choice: inflation-indexed floor with supply-side response, macroprudential discipline, and commons-layer protection.
- Cost borne by: complexity; macroprudential capacity required.
- Status: Partially resolved; macroeconomic dynamics tested in SCN-016. Open.

### CON-022 | Reform speed vs. Reform legitimacy

- Affected: VAL-005, VAL-018; ART-024, ART-025.
- Description: faster reform exploits political windows; slower reform builds legitimacy; many reforms require both speed and legitimacy.
- Resolution options: (a) fast and risk legitimacy; (b) slow and risk window; (c) sequenced "protect first, redistribute second."
- Resolution choice: sequenced approach in adoption playbook (DEC-021); foundational protections fast; redistributive and regulatory reforms phased.
- Cost borne by: those harmed by status quo who must wait; framework accepts the cost for durability.
- Status: Resolved.

### CON-023 | Behavior change at scale vs. Institutional bandwidth

- Affected: VAL-018, VAL-002, VAL-012, VAL-014; ART-007.
- Description: framework relies on long-horizon behavioral change in cooperation, trust, mental health, care behaviors, ecological consumption; institutional levers are bandwidth-limited.
- Resolution options: (a) assume rapid behavior change; (b) assume no behavior change; (c) plan for moderate-pace change with multi-decade horizon.
- Resolution choice: moderate-pace assumption with multi-decade horizon; institutional reinforcement; communication; education.
- Cost borne by: those who hoped for faster change; framework accepts this as realistic.
- Status: Resolved; behavior-change rate tracked in ASM-007 and SCN-020.

### CON-024 | Adversarial review of adversarial review

- Affected: VAL-018, VAL-006; ART-009 GOV-B5.
- Description: who audits the auditor? The adversarial-review body itself can fail.
- Resolution options: (a) no audit of GOV-B5; (b) audit by another body that itself needs audit; (c) audit by constitutional court plus public reporting plus sortition oversight.
- Resolution choice: constitutional-court review of GOV-B5 procedural compliance; public reporting; sortition body can investigate GOV-B5.
- Cost borne by: simplicity; mutual-audit chains have terminal point only at constitutional level.
- Status: Resolved; risk of GOV-B5 capture remains, tracked in ASM-001.

## Open Contradictions (not yet resolved)

- CON-008: Universal floor vs. tax-base sustainability — partial resolution; international cooperation dependent.
- CON-021: Universal floor vs. inflation — partial resolution; macroeconomic testing needed.
- Various: many TZ-XXX tradeoffs are documented but specific case applications remain to be tested.

## Maintenance

- New contradictions found by future iterations get next available ID.
- Resolutions can be revisited; status updates with rationale.
- Contradictions arising from new evidence may move from `Resolved` back to `Open`.

## Cross-References

- ART-008 Articles III and IV (tradeoff zones and conflict-resolution procedure).
- ART-027 decision log (resolutions are decisions).
- ART-028 assumption register (some resolutions depend on assumptions).
- ART-030 risk register (open contradictions are also risks).
