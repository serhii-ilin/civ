# Economic System

Artifact ID: ART-010
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: MOD-ECO
Depends on: ART-008

## Purpose

Specify the economic architecture: how production, distribution, and consumption are organized so that basic needs are secured, contribution is rewarded, concentration is constrained, ecological limits hold, and innovation continues. The design is bound by `value-constitution.md` (ART-008) and by ecological constraints in `ecology-and-infrastructure-system.md` (ART-015).

The core design choice is a **mixed economy with four layers**: a commons layer for essentials, a public-provisioning layer for universal services, a regulated market layer for most goods and services, and a discretionary market layer for luxuries and high-variance innovation. Land, finance, and ecological commons sit under a fifth, structurally separated, governance regime.

## Design Heuristics

From `evidence-matrix.md` and `failure-mode-register.md`:

- Decouple survival security from labor coercion (B-016, CLM-025; mitigates RSK-014, RSK-025, RSK-016).
- Price or constrain ecological externalities (CLM-027, CLM-072; mitigates RSK-006).
- Block political-economic concentration loops (CLM-004, CLM-021; mitigates RSK-001, RSK-024).
- Reward contribution without coercive precarity (B-012; mitigates RSK-014).
- Maintain inter-generational stewardship (VAL-016).
- Recognize care work and unpaid labor (VAL-017).
- Preserve innovation through market mechanism in non-essential domains (CLM-023 caveat).

## Five-Layer Architecture (ECO-L)

### ECO-L1 Commons Layer

Goods and services treated as commons: collectively governed, non-excludable, non-rivalrous (or made so through institutional rules), priced at zero or at production cost.

- Inclusions: drinking water at basic-needs volume; air quality; basic energy at sufficient floor; public broadcasting; primary and secondary education; basic healthcare; emergency services; public space and parks; basic transit; basic digital connectivity; primary scientific knowledge and public-research outputs.
- Governance: tier-appropriate commons councils (drawing on Ostrom design principles, CLM-010); user-fees only where conservation requires them; long-horizon investment governance.
- Financing: tax-funded; protected against budget cuts by constitutional or statutory floors.

### ECO-L2 Public Provisioning Layer

Universal services delivered through public institutions, accessed by all, financed through taxation and social insurance.

- Inclusions: full healthcare (extending the L1 minimum), full education (extending L1), eldercare, childcare, disability support, public transit at full coverage, public-interest media beyond basic broadcasting.
- Governance: public agencies under GOV-B4; performance audited by GOV-B8; user feedback through GOV-B9.
- Financing: progressive taxation and social insurance.

### ECO-L3 Regulated Market Layer

The default mode for most goods and services. Private firms, cooperatives, sole proprietors, partnerships operate under regulation that internalizes externalities and protects competition.

- Inclusions: most food, clothing, housing supply (above the L2 floor), most consumer goods, most services.
- Governance: market regulation by GOV-B10 independent regulators; antitrust active; labor protections strong; environmental compliance mandatory.
- Forms: standard for-profit firms, worker cooperatives, consumer cooperatives, B-corps, social enterprises, sole proprietors, partnerships, public-benefit corporations.

### ECO-L4 Discretionary Market Layer

A thin layer for luxuries and high-variance innovation, with lighter regulation but harder ecological and concentration limits.

- Inclusions: luxury goods, status consumption, novel technology in early stage (subject to safety), entertainment beyond public-interest provision.
- Governance: same market regulation as L3 plus luxury and externality taxes; ecological limits unchanged.
- Rationale: allows innovation and individual variation without making it the engine of the whole economy.

### ECO-L5 Structurally Separate Regimes

Three domains are governed under their own regimes because market dynamics produce systemic harm when they apply:

- **Land**: land cannot be unconditionally owned in a way that captures unearned community-generated value. Long-term leasehold, land-value taxation, community land trusts, and inheritance limits apply. (See ART-015.)
- **Finance**: the financial system is regulated as critical infrastructure with banking activity separated from speculation, leverage constrained, systemic-risk monitoring, deposit insurance, public banking option, and resolution authority.
- **Ecological commons**: air, water, biodiversity, soil, climate are governed by ecological boundaries with binding caps; permits where allowed are limited and auctioned with proceeds going to ecological-restoration fund and per-citizen dividend (variant of cap-and-dividend).

## Income, Wealth, and Distribution (ECO-I)

### ECO-I1 Universal Basic Services + Floor

A baseline of dignified survival is guaranteed via the commons (L1) and public provisioning (L2). On top of that, the framework provides a cash floor (a Universal Basic Income or near-equivalent system) sized to cover discretionary needs above provided services.

- Rationale: severs survival from labor coercion (B-016, RSK-014, RSK-025) while preserving market signals for non-essential goods.
- Funding: a combination of (a) carbon, land-value, financial-transaction, and inheritance taxation; (b) automation revenue (ECO-T4); (c) sovereign-wealth investment income.
- Indexing: floor is indexed to actual cost of living, not nominal CPI; recalculated regionally.
- Conditionality: unconditional in normal circumstances; reduced only in narrow specified cases (extended absence from polity, criminal restitution).

### ECO-I2 Earnings, Compensation, and Inequality Caps

- Pay-ratio limits within firms: firm-level maximum pay-ratio (between highest- and lowest-paid full-time worker including total compensation) of 20:1 for firms above a size threshold; smaller for firms in L1/L2 (5:1 to 10:1).
- Sectoral wage boards: tripartite (labor, employer, public) wage-floor setting by sector.
- Disclosure: total compensation including equity is disclosed for senior officers and large shareholders.
- Rationale: structural moderation of inequality (CLM-020, CLM-021); behavioral evidence on dignity and procedural fairness (B-002).

### ECO-I3 Wealth Concentration Controls

- Progressive wealth tax on net wealth above a high threshold; rate calibrated to maintain stable wealth distribution across generations (target: a ceiling on inheritability of fortunes large enough to dominate politics).
- Inheritance tax with lifetime-receipt accounting per heir (not estate-level), with progressive rates.
- Closure of trust and pass-through loopholes; international tax cooperation a foreign-policy priority.
- Rationale: prevents dynastic political power (RSK-001, RSK-004, RSK-023); supports VAL-006.

### ECO-I4 Care Work Recognition

- Time spent in primary caregiving (children, elders, disabled members) counts toward pension and social insurance.
- Direct cash transfers for caregiving roles at scale beyond family.
- Paid family leave funded through social insurance.
- Rationale: VAL-017; mitigates RSK-027.

## Taxation (ECO-T)

The tax system is designed for four objectives simultaneously: (i) revenue, (ii) externality pricing, (iii) inequality moderation, (iv) intergenerational stewardship. Tax instruments:

### ECO-T1 Income Tax

- Progressive personal income tax with a high marginal rate at the top decile.
- Capital income taxed at the same rate as labor income (parity).
- Single-payer-style information reporting; pre-filled returns.

### ECO-T2 Wealth and Inheritance Tax

- Wealth tax above high threshold (ECO-I3).
- Lifetime-receipt inheritance tax per heir.
- Trust transparency mandatory.

### ECO-T3 Land Value Tax

- Tax on unimproved land value, regionally calibrated.
- Captures community-generated rent; reduces speculation; encourages productive use.
- Rationale: classical Georgist instrument; pairs well with land-tenure reform in ART-015.

### ECO-T4 Externality Taxes

- Carbon tax with rising trajectory; revenue split between cap-and-dividend (per-citizen rebate) and transition investment.
- Pollution taxes calibrated to abatement cost.
- Water and resource withdrawals taxed above sustainable yield.

### ECO-T5 Automation and Rent Taxes

- Tax on the share of corporate value-add attributable to large-scale automation, applied to firms above a size threshold.
- Tax on monopoly rents identified through structural-economic analysis (excess returns over capital cost in concentrated industries).
- Rationale: distribute gains from automation (RSK-013 mitigation, CLM-028 framing); compensate workers displaced by labor-replacing technology.

### ECO-T6 Financial Transaction Tax

- Small tax on financial transactions; designed to discourage purely speculative high-frequency activity without burdening productive investment.

### ECO-T7 Consumption Tax

- VAT-style consumption tax with progressivity built through exemptions (essentials) and luxury surcharges (L4).
- Used carefully because of regressivity in raw form; the floor (ECO-I1) compensates.

## Money, Credit, and Banking (ECO-M)

### ECO-M1 Central Bank

- Independent central bank with constitutional mandate.
- Dual mandate: price stability and employment; with an explicit constraint to operate within ecological limits.
- Public reporting on transmission and distributional effects of monetary policy.

### ECO-M2 Banking Structure

- Commercial banking separated from speculative trading (modern Glass-Steagall-like rule).
- Capital and leverage requirements calibrated to systemic risk.
- Resolution authority for failing systemic institutions; depositors protected up to threshold.

### ECO-M3 Public Banking Option

- Public option at retail level (basic accounts, payments); national or regional public investment bank for long-horizon and counter-cyclical investment.
- Rationale: maintains floor on banking access; counter-balance to private financial concentration.

### ECO-M4 Macroprudential Regulation

- Limits on household leverage; counter-cyclical capital buffers; macroprudential supervision of shadow banking.

### ECO-M5 Currency and Cross-Border

- National currency standard; cross-border capital flows monitored; mechanisms in place to handle speculative capital flight without imposing harm on member savers.

## Markets, Antitrust, and Industrial Policy (ECO-MK)

### ECO-MK1 Antitrust

- Active antitrust authority with structural-separation powers.
- Prohibitions on cross-market dominance; required interoperability and data portability for dominant platforms.
- Periodic review of concentrated markets; default action when concentration thresholds are persistently exceeded.

### ECO-MK2 Cooperative and Worker-Owned Sector

- Cooperative formation supported through technical assistance, tax treatment, and conversion financing.
- Worker-buyout right where firms are sold or close.
- Cooperative federation infrastructure (BMK-020 patterns).

### ECO-MK3 Industrial Policy

- Mission-oriented investment in: clean energy, public health, sustainable agriculture, public-interest infrastructure, foundational research.
- Procurement-driven demand for emerging green and care-economy goods and services.
- Transparency on industrial-policy choices and outcomes; subject to GOV-B5 review.
- Rationale: CLM-023 (mission-oriented public investment can shape direction); pair with antitrust to prevent capture.

### ECO-MK4 Trade

- Open trade as default for non-essential goods.
- Strategic-reserve provisions for essentials (food, energy, medicine, semiconductors, rare-earth processing). Local production floors maintained.
- Trade agreements subject to ratification (GOV-D4); labor, environmental, and human-rights standards enforced through trade policy.

## Work, Labor, and Workplace (ECO-W)

### ECO-W1 Labor Rights

- Right to organize; collective bargaining; sectoral bargaining boards.
- Strong protections against retaliation and discrimination.

### ECO-W2 Workplace Standards

- Maximum-hour rules; paid time off including sick, parental, caregiving, civic-service leave; safety standards.
- Voice mechanisms within firms above a size threshold (works councils, board-level representation).

### ECO-W3 Transitions

- Just-transition support for workers in declining sectors: income protection, retraining, relocation assistance.
- Funded through automation and externality taxes.

### ECO-W4 Civic Service

- Paid leave for civic service (sortition participation, jury duty, election administration).
- Voluntary national-service option providing skills, social mixing, and pathway into public-service careers.

## Property and Ownership (ECO-P)

### ECO-P1 Private Ownership

- Private ownership of consumer goods, productive enterprises (subject to L3 rules), housing (subject to ECO-P3), and intellectual property (subject to ECO-P4) is recognized and protected.

### ECO-P2 Public and Common Ownership

- Public ownership of L1, much of L2, and ecological commons (subject to ECO-L5).
- Cooperatives, mutuals, and trusts encouraged in L2 and L3.

### ECO-P3 Housing Tenure

- Mixed: owner-occupied (with land lease or land-value tax), social housing, cooperative housing, regulated private rental.
- Anti-speculation measures: limits on private investor purchase, transaction surcharges, vacancy penalties.
- See ART-015.

### ECO-P4 Intellectual Property

- Patent terms shorter than current default with stricter novelty requirements.
- Mandatory licensing for essential medicines and public-health technologies.
- Public-funded research outputs default to public domain.
- Trade-secret protection bounded; algorithmic transparency overrides trade secret for high-impact public-sector use (per ART-016).

### ECO-P5 Data Ownership

- Personal data is held under member control with rights of access, portability, deletion, and revocation of consent.
- Aggregated data with no individual identification can be commons-licensed.
- See ART-016.

## Innovation and Entrepreneurship (ECO-IN)

### ECO-IN1 Public Research Infrastructure

- Sustained public funding of basic research at universities and dedicated institutions.
- Open-access publication for publicly funded research.
- Public databases and data infrastructure.

### ECO-IN2 Startup Support

- Public investment bank and regional development funds invest in early-stage ventures meeting public-benefit criteria.
- Simplified business formation; mentor and technical-assistance programs.

### ECO-IN3 Innovation Without Concentration

- Antitrust monitors for emergent concentration in new sectors.
- Periodic review of platform dynamics; required interoperability where network effects are dominant.

## Indicators (ECO-M)

The economy's performance is judged on a panel of indicators, not single-metric maximization (CLM-189):

- Material wellbeing: median real income, basic-needs coverage, housing affordability, food security, healthcare access.
- Inequality: Gini coefficient, top-decile share, wealth concentration, gender and ethnic gaps.
- Mobility: inter-generational income mobility (CLM-110), educational mobility.
- Ecological: carbon, material footprint, biodiversity, water, ecological balance vs. boundaries (VAL-003).
- Resilience: supply-chain concentration, reserve duration, employment stability, financial-system buffers.
- Innovation: research intensity, patent quality, new-firm formation, productivity in non-financial sectors.
- Wellbeing: capability index, subjective wellbeing, time-poverty, loneliness, mental-health access.
- Care: caregiver-burden distribution, paid family-leave usage, eldercare quality.
- Governance: anti-trust enforcement actions, tax-gap closure, capture-resistance audit findings.

Reports are produced annually; long-horizon trends are reviewed every five years; deviations trigger review by GOV-B4 and GOV-B5.

## Open Issues and Risks

- **Capital flight risk**: aggressive wealth and inheritance taxation interacts with cross-border capital mobility. The framework needs international cooperation; in its absence, exit-friction instruments are deployable but contested. Future iterations should specify.
- **Automation tax base shrinkage**: if value-add migrates to automated capital, the tax base shifts; the framework's automation-tax design (ECO-T5) is plausible but operationally complex.
- **Cooperative scalability**: cooperatives at large scale face capital-access and governance challenges; Mondragon (BMK-020) and others provide models but durability under stress is mixed.
- **Inflation under universal floor**: a robust floor combined with services-inflation in care sectors could pressure prices; macroprudential response and supply-side policy must be coordinated.
- **Land-value tax administration**: politically and administratively demanding; transition policy required (see ART-024).
- **Patent reform**: ECO-P4 trades off short-run innovation incentives against access; the cut points need calibration.
- **Money creation under ecological-limit constraint** (CLM-027): orthodox monetary expansion may be inconsistent with binding ecological limits; the framework's central-bank mandate (ECO-M1) requires explicit operational rules in a future iteration.

## Cross-References

- Bound by: VAL-003, VAL-013, VAL-014, VAL-016, VAL-017.
- Coordinates with: ART-015 (land, ecology), ART-012 (health financing), ART-016 (data, automation), ART-019 (simulation).
- Tested in: simulation scenarios for inequality dynamics, automation transitions, housing markets, capital flight, ecological cap binding.
