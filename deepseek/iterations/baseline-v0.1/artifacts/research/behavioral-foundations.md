# ART-007: Behavioral Foundations

Iteration: `baseline-v0.1`
Status: draft

## Purpose

Define the behavioral assumptions underlying the civilization framework. What do we assume about human nature, motivation, cooperation, conflict, trust, and decision-making? Every assumption must be stated, classified, and linked to evidence.

## Core Behavioral Model

This framework adopts a **realistic-eudaimonic** model of human behavior:

- Humans are neither purely rational self-maximizers (homo economicus) nor purely cooperative altruists (homo reciprocans), but a complex mixture of self-interest, pro-sociality, bounded rationality, and context-dependent behavior.
- Behavior is shaped by institutions, incentives, norms, and environment.
- People are capable of both extraordinary cooperation and devastating cruelty depending on structural conditions.
- Designing for the worst reasonable-case behavior is safer than relying on best-case behavior. Preventing harm through institutional design is more reliable than exhorting virtue.

## Foundational Behavioral Findings

### BF-001: Bounded Rationality

**Finding**: Human cognitive capacity is limited. People use heuristics, satisfice rather than optimize, and make systematic errors under uncertainty, time pressure, and information overload.

**Evidence Classification**: [ESTABLISHED]
**Sources**: SRC-015
**Design Implications**:
- Governance and institutional processes must account for cognitive limits.
- Complexity should be managed, not increased without corresponding support structures.
- Default options matter enormously: defaults should be pro-social and safe.
- Decisions with irreversible or catastrophic consequences require structured deliberation, not snap judgment.
- Information presentation affects decision quality: design for comprehension, not just availability.

**Used In**: MOD-GOV, MOD-LAW, MOD-TAI, MOD-ECO

---

### BF-002: Prosociality Is Conditional

**Finding**: Humans exhibit high levels of cooperation, fairness, and altruism, but these are conditional on perceptions of fairness, reciprocity, group identity, and institutional trust. People cooperate when they believe others will cooperate and that free-riders will be sanctioned.

**Evidence Classification**: [ESTABLISHED]
**Sources**: SRC-002, SRC-016, SRC-078
**Design Implications**:
- Institutions must be perceived as fair to elicit cooperation.
- Free-rider detection and graduated sanction mechanisms are necessary (Ostrom's design principles).
- Cooperation scales best when nested: small-group cooperation within larger institutional frameworks.
- Visible cooperation norms (public reporting of compliance, prosocial modeling) reinforce behavior.
- Punishment of free-riders must be proportional and consistent, not arbitrary or vindictive.

**Used In**: MOD-GOV, MOD-ECO, MOD-CUL

---

### BF-003: Trust Is Earned, Not Assumed

**Finding**: Social trust (generalized trust in strangers) is built through repeated fair interactions, transparent institutions, low corruption, and shared civic experiences. It is destroyed rapidly by betrayal, corruption, perceived unfairness, and institutional failure. Trust recovery is slow and fragile.

**Evidence Classification**: [ESTABLISHED]
**Sources**: SRC-017, SRC-076, SRC-010
**Design Implications**:
- Institutional transparency and accountability are not optional -- they are trust prerequisites.
- Trust-repair mechanisms must be built into governance (truth commissions, public acknowledgment of failure, remedy).
- Rapid-response complaint resolution prevents trust erosion from festering.
- Trust metrics should be monitored as key societal health indicators.
- Design for "trust but verify" -- trustworthiness through transparency rather than blind faith.

**Used In**: MOD-GOV, MOD-CUL, MOD-LAW

---

### BF-004: Dunbar-Scale Social Limits

**Finding**: Human social-cognitive architecture evolved for groups of approximately 150 stable relationships. Larger-scale organization requires institutional scaffolding: laws, norms, symbols, narratives, and formal roles that simulate the intimacy of small-group interaction.

**Evidence Classification**: [CONTESTED] (exact number debated; scaling principle broadly accepted)
**Sources**: SRC-014
**Design Implications**:
- Primary community units should operate at human-scale (roughly 100-300 people for face-to-face governance).
- Higher governance tiers should be federated, not monolithic.
- Institutions should "feel" personal: accessible representatives, local courts, community-level services.
- Large institutions must create small-group interfaces (neighborhood councils, community courts, local service centers).
- Digital tools should connect, not replace, face-to-face interaction.

**Used In**: MOD-CUL, MOD-GOV

---

### BF-005: Self-Determination Theory -- Autonomy, Competence, Relatedness

**Finding**: Intrinsic motivation, wellbeing, and prosocial behavior are predicted by satisfaction of three basic psychological needs: autonomy (volition and self-endorsement of actions), competence (mastery and effectiveness), and relatedness (belonging and mutual care). These needs are cross-culturally validated.

**Evidence Classification**: [ESTABLISHED]
**Sources**: SRC-016
**Design Implications**:
- Governance must provide genuine autonomy (not just token participation), including meaningful choices and real influence over collective decisions.
- Economic systems must support competence development and recognition across all contribution types, not just market-valued labor.
- Community design must foster relatedness through shared spaces, rituals, mutual-aid structures, and care networks.
- Education must be autonomy-supportive (intrinsic motivation) rather than controlling (extrinsic rewards and punishments).
- Work design should maximize autonomy, skill development, and social connection.

**Used In**: MOD-EDU, MOD-ECO, MOD-CUL, MOD-GOV

---

### BF-006: Scarcity and Cognitive Bandwidth

**Finding**: Poverty, time pressure, and resource scarcity consume cognitive bandwidth, reducing decision quality, impulse control, and long-term planning capacity. This creates self-reinforcing poverty traps independent of individual character.

**Evidence Classification**: [ESTABLISHED]
**Sources**: SRC-012, SRC-054
**Design Implications**:
- Economic security floor eliminates scarcity-tax on cognition.
- Social services must be simple to access, with proactive outreach rather than complex application processes.
- Default options should protect the cognitively overloaded (opt-out rather than opt-in for beneficial programs).
- Financial and administrative complexity should not be used as a screening mechanism for benefits.
- Universal design reduces the cognitive burden of means-testing.

**Used In**: MOD-ECO, MOD-HMH

---

### BF-007: Trauma and Behavioral Development

**Finding**: Adverse childhood experiences, toxic stress, and trauma alter neurodevelopment, stress-response systems, and behavioral patterns. Trauma exposure is prevalent in all populations, and its effects are transmitted intergenerationally. Trauma-informed environments improve outcomes across health, education, justice, and social domains.

**Evidence Classification**: [ESTABLISHED]
**Sources**: SRC-019, SRC-049
**Design Implications**:
- All institutions that interact with people (especially children, vulnerable adults, and people in crisis) should be trauma-informed by default.
- Healthcare, education, law enforcement, social services, and community spaces should adopt trauma-informed practices: safety, trustworthiness, peer support, collaboration, empowerment, cultural responsiveness.
- Prevention through universal early-childhood support, family services, and community safety is cost-effective compared to downstream remediation.
- Punitive institutional responses often re-traumatize and worsen behavioral outcomes.
- ACE screening and early intervention should be universal, not targeted (to avoid stigma).

**Used In**: MOD-HMH, MOD-EDU, MOD-LAW, MOD-CUL

---

### BF-008: Moral Pluralism and Cultural Variation

**Finding**: Moral foundations vary across cultures and individuals (care/harm, fairness/cheating, loyalty/betrayal, authority/subversion, sanctity/degradation, liberty/oppression). Political and cultural conflicts often represent different weightings of shared moral foundations rather than good vs. evil contests. WEIRD populations (Western, Educated, Industrialized, Rich, Democratic) are psychological outliers globally.

**Evidence Classification**: [ESTABLISHED] for existence of variation; [CONTESTED] for specific moral-foundations taxonomy
**Sources**: SRC-053, SRC-031
**Design Implications**:
- Value constitution must accommodate diverse moral frameworks, not impose one cultural tradition's moral intuitions on all.
- Core shared values should be thin enough for consensus but thick enough to constrain extractive or oppressive behavior.
- Cultural communities should have significant autonomy within shared constitutional bounds.
- Cross-cultural perspective-taking should be built into civic education and governance deliberation.
- Political design should avoid rewarding moral outrage entrepreneurs who profit from polarization.

**Used In**: MOD-CUL, MOD-GOV, MOD-EDU

---

### BF-009: Identity and Group Conflict

**Finding**: Group identity is deeply ingrained, easily activated, and powerfully motivating. In-group favoritism and out-group hostility can be triggered by minimal cues. However, superordinate goals, shared identity, intergroup contact under equal-status conditions, and institutional fairness reduce intergroup conflict.

**Evidence Classification**: [ESTABLISHED]
**Sources**: SRC-042, SRC-096, SRC-089
**Design Implications**:
- A shared civic identity must be cultivated alongside respect for sub-group identities.
- Institutions should promote cross-group contact and collaboration rather than sorting people into homogeneous groups.
- Electoral and governance systems should be designed to reward cross-group coalition-building rather than ethnic/identity mobilization.
- Crisis responses must be carefully designed to avoid activating intergroup hostility (scapegoating).
- Federalism and cultural autonomy can reduce zero-sum ethnic competition for state control.

**Used In**: MOD-CUL, MOD-GOV, MOD-DEF

---

### BF-010: Power Corrupts -- Structural, Not Moralistic Understanding

**Finding**: Power (control over resources, outcomes, and people) produces measurable psychological changes: reduced empathy, increased risk-taking, objectification of others, inflated self-assessment, and ethical blind spots. These are structural effects of power, not personality defects. Institutional design must constrain power regardless of the virtue of power-holders.

**Evidence Classification**: [ESTABLISHED]
**Sources**: SRC-001, SRC-011, SRC-033
**Design Implications**:
- No individual should hold unconstrained power. All authority must be limited, rotated, contestable, and auditable.
- Power-concentration metrics should be actively monitored.
- Decision-making should be distributed across multiple bodies with competing interests and different institutional incentives.
- Leader psychology testing and fitness reviews are supplements, not substitutes, for structural power constraints.
- Whistleblower protections and adversarial review bodies are necessary counterweights.

**Used In**: MOD-GOV, MOD-LAW, MOD-TAI, MOD-DEF

---

### BF-011: Status Seeking and Relative Deprivation

**Finding**: Humans care intensely about relative position, not just absolute wellbeing. Status competition is a powerful motivator that can drive innovation and achievement or fuel destructive arms races in consumption, political power, and identity conflict. Perceived unfairness in status distribution produces grievance, unrest, and violence.

**Evidence Classification**: [ESTABLISHED]
**Sources**: SRC-050, SRC-046, SRC-047
**Design Implications**:
- Reduce the stakes of status competition: compress the material distance between top and bottom.
- Provide multiple, non-convertible status hierarchies (excellence in art, science, community service, craft, care, public service) rather than a single currency (money, power).
- Status based on contribution to shared values is healthier than status based on extraction or domination.
- Visible inequality generates resentment and degrades social trust independent of absolute poverty levels.
- Luxury consumption and positional-goods arms races should be taxed and discouraged through social norms rather than prohibition.

**Used In**: MOD-ECO, MOD-CUL, MOD-GOV

---

### BF-012: Generational Cultural Transmission

**Finding**: Values, norms, and identity are transmitted across generations through families, education, rituals, media, and institutional experiences. Transmission fidelity is imperfect: each generation reinterprets and adapts. Founding commitments attenuate without active renewal. Cultural transmission breaks down when institutions lose perceived legitimacy or when economic/social conditions make inherited norms non-adaptive.

**Evidence Classification**: [ESTABLISHED]
**Sources**: SRC-031, SRC-042
**Design Implications**:
- Civic education must transmit shared values without indoctrination -- teaching why institutions exist, not just that they should be obeyed.
- Intergenerational institutions (mentorship programs, community rituals, shared governance bodies) build transmission bridges.
- Founding narratives must be inclusive, honest about historical failures, and oriented toward future aspirations.
- Generational-commitment metrics should be monitored: do young adults share civic commitments?
- Institutional renewal mechanisms (periodic constitutional conventions, citizen assemblies) refresh consent.

**Used In**: MOD-EDU, MOD-CUL, MOD-GOV

---

### BF-013: Behavioral Design and Choice Architecture (Nudge-Like Effects, With Ethical Constraints)

**Finding**: The way choices are presented -- defaults, framing, salience, social norms, simplification -- strongly influences behavior without restricting choice. Nudge-like designs can promote prosocial behavior and public health at low cost. However, they raise ethical concerns about manipulation, lack of transparency, and potential misuse by authorities.

**Evidence Classification**: [ESTABLISHED] for effectiveness; [CONTESTED] for ethical framework
**Sources**: SRC-030, SRC-015
**Design Implications**:
- Defaults should be pro-social, pro-health, and pro-environmental (opt-out rather than opt-in for beneficial programs).
- Choice architecture must be transparent: people should understand how choices are structured and by whom.
- Manipulative design (dark patterns) must be prohibited by law for public institutions and regulated for private entities.
- Behavioral design requires adversarial review: who benefits, who is nudged, toward what end?
- Nudge-like designs are complements to, not substitutes for, structural fairness.

**Used In**: MOD-GOV, MOD-LAW, MOD-TAI, MOD-HMH

---

## Behavior Under Institutions: The Interaction Model

The civilization design assumes that institutions and individual behavior co-evolve:

1. **Institutions shape behavior**: Fair, transparent, competent institutions produce trusting, cooperative, prosocial citizens. Extractive, opaque, corrupt institutions produce defensive, self-interested, low-trust citizens.

2. **Behavior shapes institutions**: Cooperative citizens sustain good institutions through participation, norm enforcement, and political support. Defensive citizens cannot sustain good institutions because collective action fails.

3. **Path dependency**: Early institutional design choices lock in behavioral patterns. A society that starts with fair, transparent institutions is easier to maintain than one that must reform after corruption is normalized.

4. **Crisis dynamics**: Institutional trust is a stock that depletes rapidly in crisis but accumulates slowly in normal times. Repeated crises with competent response build resilience; repeated crises with incompetent response destroy it.

5. **Heterogeneity**: Individual variation in cooperativeness, risk tolerance, time preference, and other traits is substantial. Institutional design must work for the 90th percentile of selfishness, not the 50th percentile.

## Unresolved Behavioral Questions

These questions are carried forward to module-level design and remain open for future iteration:

1. **UBHQ-RES-001**: What is the minimum viable proportion of cooperators in a population for prosocial institutions to be stable? (Evidence suggests 30-50%, but context-dependent.)
2. **UBHQ-RES-002**: How does behavior adapt to abundance vs. scarcity? Does universal basic provisioning change baseline cooperation, effort, and creativity, or only remove precarity constraints?
3. **UBHQ-RES-003**: What is the interaction between institutional design and personality structure? Do institutions select for or against certain personality traits over generations?
4. **UBHQ-RES-004**: How stable are cultural values under sustained external pressure (economic competition, military threat, information warfare)?
5. **UBHQ-RES-005**: What is the maximum sustainable rate of institutional change without disrupting behavioral adaptation capacity?

These questions should be revisited with simulation results in future iterations.