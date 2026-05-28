# Assumption Register

Artifact ID: ART-028
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: all

## Purpose

Record every load-bearing assumption that the framework makes but cannot fully validate from the evidence available. Each assumption is tagged with the artifact(s) that depend on it, a test method, a failure signal, and current status.

The intent is operational: if an assumption fails, the framework should know which design choices to revisit. Assumptions are not necessarily wrong; they are unfinished. Some may move to `validated` if simulation, pilot, or new evidence supports them; some may move to `falsified` if evidence breaks them.

## Format

```text
ASM-XXX | Statement | Used In | Test Method | Failure Signal | Status
```

## Assumptions

| Assumption ID | Statement | Used In | Test Method | Failure Signal | Status |
| --- | --- | --- | --- | --- | --- |
| ASM-001 | Standing adversarial-review bodies can maintain independence across decades. | ART-009 GOV-B5, ART-018 TAR-P6 | Simulation SCN-001, SCN-012; historical comparison with auditors-general and ombudsmen in long-running cases. | Adversarial-review body itself captured or starved; investigative output drops. | Open |
| ASM-002 | Sortition bodies retain legitimacy at large scale and over years, not only at single events. | ART-009 GOV-B1, GOV-B6 | SCN-019; pilot programs in real polities. | Sortition output systematically dismissed; participation collapses; capture observed. | Open (CLM-018 contested) |
| ASM-003 | Pay-ratio caps within firms do not produce equilibrium-defeating fragmentation. | ART-010 ECO-I2 | Simulation runs; case study (BMK-020 Mondragon mixed evidence). | Fragmentation rate observed; productive activity moves outside the cap regime. | Open |
| ASM-004 | Universal floor + commons does not trigger inflation collapse under normal conditions. | ART-010 ECO-I1 | SCN-016; macroeconomic modeling. | Inflation un-anchored; real value of floor collapses; basic-needs affordability declines despite floor. | Open |
| ASM-005 | Land-value taxation is administrable at national scale with current cadastral technology. | ART-010 ECO-T3, ART-015 ECN-L1 | Pilot programs; international experience (BMK-008 Uruguay, Estonia and others). | Assessment costs exceed revenue; politically captured to neutralize. | Open |
| ASM-006 | Hard ecological caps can be politically maintained across electoral cycles. | ART-015 ECN-B1 | SCN-005, SCN-020 long-horizon; observed compliance vs. trajectory. | Cap-breaching becomes routine; political-economy default to relaxation. | Open |
| ASM-007 | Behavioral institutional design (procedural fairness, autonomy support, trauma-informed default) shifts population-level indicators in 1-2 generations. | ART-007, ART-012, ART-013, ART-014 | Long-horizon indicator tracking; SCN-011, SCN-020. | Indicators flat or worsen despite institutional changes; behavioral mechanisms swamped by other factors. | Open |
| ASM-008 | Cryptographic separation of personal data and observability infrastructure is technically and operationally maintainable. | ART-016 TAI-O6, DEC-020 | Security audits; SCN-014 observability creep. | Repeated separation failures; surveillance creep documented; technical means inadequate. | Open |
| ASM-009 | AI risk classification (TAI-R) keeps pace with capability trajectory. | ART-016 | Continuous regulatory-evaluation review; international coordination. | High-risk systems emerge faster than regulation updates; harms accumulate. | Open |
| ASM-010 | Coalition politics can sustain reform across at least two electoral cycles where Mode B is adopted. | ART-024, ART-025, ART-026 | Real-polity adoption tracking; coalition-survival metrics. | Coalition collapses; reforms reversed before consolidation. | Open |
| ASM-011 | Public-service media remains independent of executive capture given the framework's design rules. | ART-009 GOV-B10, ART-014 CUL-MI1 | Press-freedom indicators; SCN-002 demagogue ascent variations. | Public broadcaster captured or defunded. | Open |
| ASM-012 | Judicial independence under mixed-body nomination is at least as strong as under current default appointment regimes. | ART-009 GOV-B3, ART-011 LAW-C2-C3 | Comparative judicial-independence indices; SCN-002. | Captured court; rulings systematically deferential to executive. | Open |
| ASM-013 | Restorative justice scales without quality dilution for eligible offense categories. | ART-011 LAW-CJ3 | Outcomes by program type; victim-satisfaction surveys; reoffending rates. | Outcomes diverge from pilot-scale to mainstream-scale. | Open (CLM-091 variable) |
| ASM-014 | Mental-health workforce can scale to universal access in 10-15 years given investment. | ART-012 HEA-W1, HEA-M | Workforce-pipeline tracking; access-wait-time metrics. | Wait times remain above thresholds; workforce shortage persists. | Open |
| ASM-015 | Tertiary education at low or no cost does not collapse quality or distort student composition. | ART-013 EDU-P5, EDU-H3 | International experience; outcome and composition data. | Quality declines below comparable systems; mobility does not improve. | Open |
| ASM-016 | Capability-based assessment can substitute for high-stakes standardized testing in selection. | ART-013 EDU-A2-A3 | Adoption-polity outcome data; equity audits. | Selection becomes opaque or biased; mobility does not improve. | Open |
| ASM-017 | Inter-cell mobility is preserved under cell-level governance autonomy. | ART-014 CUL-I2 | Mobility data across cells; ombuds complaints. | Cells erect informal barriers; mobility collapses. | Open |
| ASM-018 | Cooperative-sector growth is feasible without permanent subsidy. | ART-010 ECO-MK2 | Cooperative-formation data; cooperative survival rates. | Cooperatives unable to compete without continuous subsidy; sector stagnates. | Open |
| ASM-019 | Tax administration can implement wealth, inheritance, automation, and land-value taxes simultaneously without overwhelming capacity. | ART-010 ECO-T | Capacity-build tracking; tax-gap metrics. | Tax administration overwhelmed; compliance gaps widen. | Open |
| ASM-020 | International cooperation on tax, AI, climate, biosecurity is achievable in relevant time-frames. | ART-010 ECO-T2, ART-016 TAI-IC, ART-015 ECN-B, ART-017 DEF-F | Treaty progress; coordination cases. | International cooperation insufficient; unilateral measures inadequate. | Open |
| ASM-021 | Civic literacy and capability outcomes can be measured without inducing teaching-to-the-test. | ART-013 EDU-A1-A2 | Audit of assessment-induced curricular narrowing. | Sampled assessments produce predictable gaming despite design intent. | Open |
| ASM-022 | Decision-log discipline can be sustained at the volume of public-body decisions. | ART-009 GOV-O1, ART-016 TAI-O1 | Audit findings; completeness metrics. | Decision logs become boilerplate, hide substantive reasoning. | Open |
| ASM-023 | Civilian-control of public-safety multi-modal response model is safe for civilian responders at scale. | ART-011 LAW-P2 | Incident data; responder safety metrics. | Civilian responders harmed at rates beyond preventable; rollback pressure. | Open |
| ASM-024 | Energy transition is feasible at the required pace within the framework's ecological budget. | ART-015 ECN-E | Transition tracking; emissions trajectory. | Pace insufficient; emissions trajectory off. | Open |
| ASM-025 | Care work recognition (cash, pension credit, time) does not produce caregiver retreat from labor market in unintended ways. | ART-010 ECO-I4, ART-014 CUL-CA1 | Labor-market data; gender-disaggregated outcomes. | Care recognition entrenches gendered specialization. | Open |
| ASM-026 | Constitutional amendment procedure can be used at the framework's recommended cadence without sclerosis or excess churn. | ART-008 Article V | Amendment-pass rates; amendment-quality assessment. | Either no amendments pass (sclerosis) or destabilizing volume passes. | Open |
| ASM-027 | Sortition-confirmed referenda do not collapse into majoritarian abuse of minorities. | ART-009 GOV-D1, GOV-D2 | Referenda outcomes; minority-rights audit. | Referenda systematically harm minorities; courts unable to constrain. | Open |
| ASM-028 | The framework's external interfaces (DEF-B) can be audited without disclosing operational-security details that undermine them. | ART-017 DEF-B8 | Audit-report quality; security-leak incidents. | Audit either uninformative (protecting too much) or leaks (protecting too little). | Open |
| ASM-029 | The framework can attract sufficient public-service workforce given pay and conditions. | ART-009, ART-012, ART-013 | Recruitment and retention data. | Public-service shortage; quality declines. | Open |
| ASM-030 | Pluralism + universal-rights enforcement can coexist with strong cultural-community self-governance. | ART-008 TZ-006, ART-014 CUL-P | Disputes between cultural communities and universal rights; resolution patterns. | Either rights regularly violated within communities, or communities chafe against universal rights leading to exit pressure. | Open |
| ASM-031 | Algorithmic-impact-assessment regimes catch most high-impact harms before deployment. | ART-016 TAI-AC3 | Post-deployment harm audit; assessment-quality review. | Major harms missed; AIA process becomes ceremonial. | Open |
| ASM-032 | Civil-defense and reserve infrastructure remains operational without acute crisis to keep it sharp. | ART-017 DEF-D, ART-015 ECN-IC | Drill outcomes; equipment readiness; reserve audits. | Atrophy in peacetime; underprepared for actual crisis. | Open |
| ASM-033 | Member-observability infrastructure does not become surveillance of members. | ART-008 TZ-004, ART-016 TAI-O7 | SCN-014; audit findings. | Surveillance creep documented; member observability of self becomes surveillance by institutions. | Open |
| ASM-034 | Long-horizon impact statements influence decisions, not just record them. | ART-009 GOV-B7, GOV-D3 | Statement-versus-decision tracking; comparison with statement-less control. | Statements ceremonial; decisions unaffected. | Open |
| ASM-035 | Public-service AI prohibitions (TAI-R2) do not push the same uses into private-sector applications with the same harms. | ART-016 TAI-R2 | Cross-sector harm tracking. | Harms shift, not reduce. | Open |
| ASM-036 | Restitution to ecological commons (under ecocide and environmental crime) produces actual restoration. | ART-011 LAW-CJ6, ART-015 ECN-B5 | Restoration-outcome audits. | Funds raised, restoration not achieved. | Open |
| ASM-037 | The framework's claim of universality holds across non-WEIRD populations. | All architecture | Adoption-pilot outcomes across cultural contexts. | Outcomes diverge significantly across contexts; framework must be revised regionally. | Open (CLM-060 caveat) |
| ASM-038 | Reform fatigue can be managed across a decade of significant institutional change. | ART-024, ART-025 | Public-support tracking; coalition stability. | Support declines below coalition viability; reforms stall or reverse. | Open |
| ASM-039 | The framework's reserve-duration targets (food, energy, medicine) are achievable without producing perpetual surplus disposal. | ART-015 ECN-IC2 | Reserve-management economics; waste-disposal metrics. | Reserves either insufficient or chronically wasted in cycling. | Open |
| ASM-040 | Naturalization criteria (DEF-MIG4) do not produce de facto exclusion of low-income migrants. | ART-017 DEF-MIG4 | Naturalization-rate by income; integration outcomes. | Naturalization stratifies by income. | Open |

## Maintenance

- Each assumption's status is updated by future iterations based on simulation, pilot, or new evidence.
- New assumptions added during iterations get the next available ID.
- Assumptions moved to `validated` or `falsified` remain in the register with status updated; entries are not deleted.
- Cross-references between assumptions and decisions (DEC-XXX) and risks (RSK-XXX) should be maintained.

## Cross-References

- ART-027 decision log: many decisions made under specific assumptions here.
- ART-029 contradiction register: where contradictions exist between assumptions, the more conservative is preserved until resolved.
- ART-030 risk register: assumption failures generate risks tracked there.
- `evidence-matrix.md` (ART-004): supporting and counter-evidence for assumptions.
