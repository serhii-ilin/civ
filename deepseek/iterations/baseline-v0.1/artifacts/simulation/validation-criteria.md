# ART-022: Validation Criteria

Iteration: `baseline-v0.1`
Status: draft

## Purpose

Define what constitutes a validated framework. Specify thresholds, red lines, tradeoff zones, and the evidence standard for declaring the design adequate, in need of revision, or fundamentally flawed.

## Validation Framework

Three levels:
1. **Internal Validation**: Does the framework satisfy its own requirements? (claims sourced, contradictions documented, logic consistent)
2. **Simulation Validation**: Does the framework survive stress testing in computational models?
3. **External Validation**: Validation against historical comparison, expert review, and pilot implementation.

---

## Level 1: Internal Validation

| Criterion | Requirement | Pass Threshold |
| --- | --- | --- |
| I-1: Claim Classification | All empirical claims classified | >95% coverage |
| I-2: Source Coverage | [ESTABLISHED] and [CONTESTED] claims cite sources | >90% sourced |
| I-3: Assumption Registration | Key assumptions in register with test method | All inter-module assumptions documented |
| I-4: Decision Documentation | Major design choices in decision log | Architecture decisions documented |
| I-5: Contradiction Documentation | Known contradictions documented with resolution options | All known contradictions documented |
| I-6: Value Compliance | Institutional designs reference applicable values | No undocumented value violations |
| I-7: Failure Mode Coverage | Failure modes addressed by mitigations | All severity >6 modes have mitigations |

---

## Level 2: Simulation Validation

### Thresholds

| Zone | Classification | Implication |
| --- | --- | --- |
| Green | Design Validated | Proceed to Level 3 |
| Yellow | Design Requires Adjustment | Targeted iteration |
| Red | Design Failure | Fundamental redesign |

### Criteria

| # | Criterion | Metric | Green | Yellow | Red |
| --- | --- | --- | --- | --- | --- |
| S-1 | Wellbeing Stability | Multidimensional Wellbeing Index | Stable/improving >80% runs | Decline >10% in >30% runs | Decline >25% in >30% runs |
| S-2 | Inequality Containment | Wealth Gini | <0.40 >80% runs | >0.45 >30% runs | >0.55 >30% runs |
| S-3 | Institutional Trust | Mean trust-in-institutions | >0.50 >80% runs | <0.40 >30% runs | <0.25 >30% runs |
| S-4 | Ecological Compliance | Boundaries transgressed (0-9) | 0-1, recovering | 2-3, no recovery | 4+, tipping cascade |
| S-5 | Corruption Containment | Corruption index | <0.10 >80% runs | >0.15 >30% runs | >0.25 >30% runs |
| S-6 | Democratic Resilience | Backsliding index | >0.70 >80% runs | <0.50 >30% runs | <0.30 >30% runs |
| S-7 | Shock Recovery | Time to 90% pre-shock | <5yr severe / <10yr catastrophic | 5-15yr | >15yr or never |
| S-8 | Generational Sustainability | Civic engagement vs. founding | >70% after 3+ gens | 40-70% | <40% |
| S-9 | Participation Robustness | Electoral + non-electoral | >60% >80% runs | 35-60% | <35% |
| S-10 | Care Infrastructure | Care-gap index | <10% >80% runs | 10-25% | >25% |

### Composite Score
- **Pass**: All 10 Green
- **Conditional Pass**: 7-9 Green, remainder Yellow, no Red
- **Fail**: Any Red

---

## Redesign Triggers

1. Any criterion Red
2. Two or more stress scenarios produce Framework Collapse
3. Fundamental contradiction cannot be resolved
4. Core value constitution internally inconsistent
5. Expert/adversarial review identifies fatal flaw

## Iteration Triggers

Targeted iteration (module_update) triggered by:
1. Conditional Pass (Yellow criteria)
2. One stress scenario produces Framework Collapse
3. New evidence materially changes [CONTESTED] or [THEORETICAL] claims
4. Simulation improvements enable testing previously untestable assumptions