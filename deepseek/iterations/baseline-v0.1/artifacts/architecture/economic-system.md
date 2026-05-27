# ART-010: Economic System Architecture

Iteration: `baseline-v0.1`
Status: draft

## Purpose

Design an economic system that secures basic needs, rewards diverse contributions, prevents extreme concentration, operates within ecological boundaries, and recognizes care work and unpaid labor as economically real.

## Core Design Principles

The economic system is organized as a **commons-centered, market-hybrid economy** with four interacting layers:

1. **Commons Layer**: Essential goods and services provided universally
2. **Cooperative Market Layer**: Market activity organized primarily through cooperatives, social enterprises, and stakeholder-governed firms
3. **Entrepreneurial Layer**: Innovation, startups, and competitive markets with strong anti-monopoly constraints
4. **Care and Reproduction Layer**: Formally recognized and supported care economy

## Layer 1: Commons Layer (Universal Basic Services)

### Scope
Essential goods and services provided universally, free at point of use or heavily subsidized:

**Provisioning Model**: Direct public provision, regulated public utilities, or regulated non-profit providers. No for-profit provision of commons-layer services.

| Service | Provisioning Model | Funding Mechanism |
| --- | --- | --- |
| Healthcare (all tiers including mental health) | Public provision + regulated non-profit clinics/hospitals | Progressive taxation + health levy |
| Education (early childhood through tertiary + lifelong) | Public provision + regulated non-profit institutions | General revenue + education levy |
| Housing (basic shelter guarantee) | Social housing + housing cooperatives + housing vouchers for private rental | Land-value tax + general revenue |
| Nutritious food (basic food security) | Community food programs + food assistance + school meals + senior meals | Agricultural subsidies redirected + general revenue |
| Water and sanitation | Public utility | User fees (basic allowance free) + cross-subsidization |
| Energy (basic allowance) | Public/cooperative utility | Progressive pricing + general revenue |
| Public transport | Public/cooperative provision | Land-value capture + user fees (basic access free) |
| Digital access (broadband, devices, digital literacy) | Public infrastructure + regulated private providers | Universal-service fund + general revenue |
| Care services (childcare, eldercare, disability support) | Public provision + regulated non-profit + family-care compensation | General revenue + care levy |

### Design Features

**Universal, not means-tested**: Universality builds political coalitions (Nordic model lesson -- BCM-005), reduces stigma, eliminates cognitive burden of applications (BF-006), and prevents poverty traps from benefit cliffs.

**Opt-out, not opt-in**: Default enrollment in all universal services. Citizens may decline services but must actively opt out, not overcome barriers to opt in.

**Quality floors**: Universal services must meet quality standards that the middle class would accept, preventing the "poor services for poor people" dynamic that undermines political support.

**Evidence**: CLM-028 (UBS vs UBI debated); CLM-022 (universal healthcare); BCM-005 (Nordic model). Sources: SRC-013, SRC-099, SRC-054.

**Decision**: DEC-ECO-001 (Universal Basic Services over Universal Basic Income). Rationale: UBS directly guarantees specific welfare outcomes (health, education, housing, nutrition) where UBI leaves outcome to market capacity and individual circumstance. UBS builds shared infrastructure; UBI provides cash without structural change. Combination approach under study for future iteration.

---

## Layer 2: Cooperative Market Layer

### Ownership and Governance Structures

The economy's default organizational form is **stakeholder-governed enterprise**:

1. **Worker cooperatives** (Mondragon model -- BCM-007): Worker-owned, one-worker-one-vote governance, profit-sharing, capped internal pay ratios.
2. **Multi-stakeholder cooperatives**: Ownership shared among workers, consumers, and community representatives.
3. **Consumer cooperatives**: Member-owned retail, housing, insurance, and financial services.
4. **Producer cooperatives**: Small-producer collective marketing, purchasing, and processing (agricultural, artisan).
5. **Community interest companies / B Corporations**: Enterprises with legally binding social/environmental mission, stakeholder governance, and profit constraints.
6. **Public-benefit corporations**: State-owned or partially state-owned enterprises for natural monopolies and strategic industries.

### Market Structure Rules

- **Anti-monopoly**: Competition authority with structural-separation powers (can break up firms). Market-share caps by sector (e.g., no firm >25% of any essential-goods market).
- **Interoperability mandates**: Essential platforms and networks must support data portability, interoperability, and third-party access.
- **Algorithmic pricing oversight**: Algorithmic price coordination treated as illegal collusion.
- **Predatory pricing prohibition**: Below-cost pricing by dominant firms to eliminate competitors is prohibited and prosecuted.

### Cooperative Ecosystem Support

- **Cooperative Development Bank**: Publicly capitalized bank providing patient capital, technical assistance, and conversion financing for enterprises transitioning to cooperative ownership.
- **Cooperative conversion incentives**: Tax incentives and technical support for retiring business owners to sell to workers rather than competitors or private equity.
- **Public procurement preference**: Cooperatives and social enterprises receive preference in public procurement (tied to quality and price parity).
- **Cooperative secondary market**: Market for cooperative shares, enabling worker liquidity without external ownership.

**Evidence**: CLM-002 (commons governance); BCM-007 (Mondragon); BCM-005 (Nordic model coordination). Sources: SRC-002, SRC-008.

**Decision**: DEC-ECO-002 (cooperative default model). Rationale: Worker ownership aligns incentives (BF-002), reduces inequality (CLM-004), and provides employment stability (BCM-007 survived 2008 crisis better than conventional firms). Traditional corporations permitted but face progressively higher tax rates above certain size and pay-ratio thresholds.

---

## Layer 3: Entrepreneurial and Innovation Layer

### Design

- **Innovation commons**: Publicly funded basic research (R&D at 3% of national income -- CLM-048) with open-access publication requirements.
- **Patent reform**: Shorter patent terms (10 years from filing, down from 20), higher non-obviousness standards, compulsory licensing for essential technologies (pharmaceuticals, climate tech), government march-in rights for publicly funded research.
- **Startup ecosystem**: Public venture-capital funds (patient capital), regulatory sandboxes, simplified incorporation, innovation prizes for public-interest challenges.
- **Small-business support**: Simplified regulation, cooperative conversion pathway, local procurement preferences.

### Anti-Monopoly for Innovation

- **Killer-acquisition review**: Acquisitions of startups by dominant firms for the purpose of eliminating competitive threats are prohibited.
- **Data-as-barrier**: Data hoarding by dominant platforms treated as barrier to entry; data-portability and interoperability mandates apply.
- **Self-preferencing prohibition**: Platforms that serve as marketplace AND seller may not preference their own products.

**Evidence**: CLM-048 (R&D investment); SRC-063, SRC-064.

---

## Layer 4: Care and Reproduction Economy

### Recognition

The care economy -- childcare, eldercare, disability care, healthcare, education, domestic labor, community maintenance, emotional labor -- is formally recognized in:

- **National economic accounts**: GPI and satellite care-economy accounts measure and value care work.
- **Social security credits**: Caregiving years count toward public pension/social-security entitlement.
- **Labor law**: Care workers (paid and unpaid) have explicit rights: leave, flexible work, anti-discrimination protections.

### Support Infrastructure

- **Universal childcare**: Free, high-quality childcare from 6 months to school age.
- **Universal pre-K**: Free preschool from age 3.
- **Paid parental leave**: 12 months per child, divided between parents with "use it or lose it" provisions for each parent to encourage equitable sharing.
- **Paid family leave**: For eldercare, disability care, and major family health events.
- **Caregiver tax credit**: For unpaid family caregivers providing substantial care.
- **Respite care**: Guaranteed respite for caregivers (paid and unpaid).
- **Community care networks**: Neighborhood-level care coordination, mutual-aid infrastructure, and elder/disabled-community integration.

**Evidence**: CLM-009 (ACEs prevention); CLM-017 (care work as infrastructure -- VAL-017). Sources: SRC-019, SRC-018.

**Decision**: DEC-ECO-003 (care economy as infrastructure). Rationale: Care work is the foundation that enables all other economic activity. Treating it as externalized cost creates gender inequality, caregiver burnout (RSK-015), and intergenerational harm (CLM-009). Formal recognition and support aligns with VAL-017.

---

## Taxation Architecture

### Principles
- **Progressivity**: Effective tax rate increases with ability to pay.
- **Ecological alignment**: Tax what we want less of (pollution, resource extraction, land speculation, monopoly rents), not what we want more of (labor, productive investment, innovation).
- **Transparency**: Each citizen receives an annual tax receipt showing what their taxes fund.
- **Simplicity**: Tax compliance should not require paid intermediaries for standard situations.

### Tax Structure

| Tax | Rate/Structure | Rationale |
| --- | --- | --- |
| Land Value Tax (LVT) | Progressive, based on unimproved land value. Owner-occupied primary residence exemption up to median land value. | CLM-014: efficient (no deadweight loss), captures socially created value. Georgist principle (BCM-014). Discourages land speculation. Sources: SRC-062, SRC-008. |
| Progressive Income Tax | Marginal rates: 0% (below basic-income threshold), 20-25% (middle), 40-50% (high), 55-60% (very high). Combined individual + capital income (no separate lower rate for capital gains). | Redistributive function. Taxing capital gains at lower rates than labor income is regressive and economically distortive (CLM-004). |
| Wealth Tax | 1-2% annually on net wealth above high threshold (e.g., top 0.1-1%). Primary-residence exemption up to median value. Retirement-account exemption up to reasonable limit. | Addresses wealth concentration (CLM-004). Valuation challenges recognized; phased implementation with improved valuation methodology. |
| Carbon and Ecological Tax | Carbon price rising to social cost of carbon. Border carbon adjustment. Material extraction tax. Pollution taxes on NOx, SOx, particulates, water pollution, chemical releases. | Internalizes ecological externalities (VAL-003). Revenue partially recycled as per-capita dividend to offset regressive effects. |
| Automation and Data Tax | Tax on revenue attributable to automation of previously human-performed labor. Data-extraction levy on large-scale personal-data harvesting. | CLM-017, CLM-018. Captures automation rents and data-extraction externalities for public benefit. Revenue funds reskilling and transition support. |
| Financial Transactions Tax | 0.1-0.5% on securities, derivatives, and currency transactions. | Reduces high-frequency speculative trading (economic activity of questionable social value). Revenue modest but behavioral effect significant. |
| Inheritance Tax | Progressive, with high exemption (e.g., median lifetime earnings). Family farm and small-business continuation exemptions. | Prevents dynastic wealth concentration (CLM-004). High exemption ensures middle-class families unaffected. |
| Sin/Pigouvian Taxes | Alcohol, tobacco, sugar, gambling, pollution above cap. | Health and ecological alignment. Revenue earmarked for prevention and treatment. |
| Corporate/Enterprise Tax | Moderate base rate. Lower rate for cooperatives and B Corps. Higher rate for enterprises exceeding pay-ratio caps or market-share thresholds. | Incentivizes cooperative and stakeholder-governance forms. Higher-rate band is anti-monopoly and anti-concentration mechanism. |
| Value-Added Tax / Consumption Tax | Moderate rate. Exemptions for basic food, medicine, education, and other essentials. | Broad consumption base with progressivity through essential exemptions. |

**Decision**: DEC-ECO-004 (tax architecture). Rationale: Tax mix follows principle of "tax bads, not goods." Ecological taxes and land-value taxes are economically efficient. Progressive income, wealth, and inheritance taxes address concentration. Tax structure broadly progressive in incidence.

---

## Wealth and Income Distribution Mechanisms

### Concentration Limits
- **Executive-to-worker pay ratio cap**: 20:1 for enterprises with government contracts or above size threshold. Exceeding ratio triggers progressive penalty tax up to confiscatory levels beyond 50:1.
- **Maximum wealth mechanism**: Not a hard cap but a combination of progressive wealth tax, inheritance tax, and anti-monopoly enforcement that makes extreme concentration unsustainable.
- **Wealth floor**: Universal basic services ensure no one falls below minimum wellbeing threshold.
- **Asset-building**: Universal child trust accounts (baby bonds) funded at birth, accessible at adulthood. Cooperative homeownership support. Worker-ownership incentives.

### Automation and Transition
- **Automation Dividend**: Revenue from automation/data taxes distributed as per-capita dividend OR invested in universal services -- allocation determined by National Assembly.
- **Job guarantee of last resort**: Community-service employment at living wage for anyone seeking work not available in private/cooperative market. Includes training and transition support.
- **Reskilling entitlement**: Every adult entitled to 2 years of publicly funded retraining/education across lifetime.
- **Reduced working time**: Policy direction toward shorter standard work week (30-35 hours) as productivity increases, maintaining living standards.

**Decision**: DEC-ECO-005 (automation response). Rationale: CLM-017 suggests significant labor disruption. Proactive transition policy (reskilling + reduced hours + dividend) is more humane and economically efficient than reactive unemployment + retraining after displacement.

---

## Monetary and Macroeconomic Policy

### Institutional Design
- **Independent Central Bank**: Mandate includes (a) price stability, (b) full employment, (c) financial stability, and (d) ecological-risk assessment. Governance by diverse board including labor, cooperative, ecological, and regional representatives.
- **Public digital currency**: Central bank digital currency (CBDC) as universal public-payment infrastructure. Private payment systems operate on CBDC rails with interoperability mandate.
- **Macroprudential regulation**: Counter-cyclical capital buffers, loan-to-value limits, debt-to-income limits to prevent asset bubbles and financial crises.
- **Public banking infrastructure**: Postal banking, community development banks, green investment bank, cooperative development bank.

### Fiscal Rules
- **Counter-cyclical fiscal policy**: Deficit spending during recessions, surplus during booms.
- **Investment budgeting**: Capital expenditure separated from operating expenditure in government accounts.
- **Intergenerational accounting**: Long-term fiscal sustainability reporting including ecological liabilities and infrastructure-maintenance obligations.
- **Debt management**: Public debt primarily domestically held, denominated in national currency.

**Decision**: DEC-ECO-006 (central-bank mandate). Rationale: Adding employment, financial-stability, and ecological-risk mandates follows post-2008 consensus that price stability alone is insufficient. CBDC provides public alternative to private payment monopolies.

---

## Evidence and Assumptions

### Key Evidence Claims Used

| Claim ID | Application |
| --- | --- |
| CLM-001 | Institutional design for inclusive economy |
| CLM-002 | Cooperative and commons governance design |
| CLM-004 | Progressive taxation and wealth-concentration limits |
| CLM-006 | Universal services to eliminate scarcity tax on cognition |
| CLM-008 | Worker ownership supporting autonomy and competence needs |
| CLM-015 | Inequality-harm relationship (with contestation noted) |
| CLM-027 | Beyond-GDP metrics adoption |
| CLM-028 | UBS effectiveness (contested, but evidence base favors services + cash hybrid) |
| CLM-044 | Circular economy design |
| CLM-048 | R&D public investment |

### Key Assumptions

| Assumption ID | Statement | Test Method | Failure Signal |
| --- | --- | --- | --- |
| ASM-ECO-001 | Universal Basic Services produce better outcomes than equivalent cash transfers for essential goods | Comparative simulation; pilot studies of UBS vs UBI | UBS delivery quality degrades below market; citizen satisfaction lower than with cash |
| ASM-ECO-002 | Cooperative enterprises can achieve productivity parity with conventional firms in most sectors | Productivity benchmarking; data collection from cooperative sectors globally | Productivity gap >15% sustained over 5+ years |
| ASM-ECO-003 | Land Value Tax can capture sufficient revenue without excessive valuation disputes or economic distortion | Simulation; analysis of existing LVT jurisdictions (Pennsylvania, Denmark, Estonia) | Valuation disputes consume >5% of tax revenue; assessment appeals exceed 10% of properties |
| ASM-ECO-004 | Progressive tax structure does not cause capital flight exceeding manageable levels | Simulation; historical analysis of tax regimes and capital mobility | Capital/wealth outflows exceed 2% of GDP per year |
| ASM-ECO-005 | Automation will produce net labor displacement requiring transition policy (magnitude and timing uncertain) | Technology-trend monitoring; labor-market forecasting; simulation | If automation creates more jobs than it displaces AND transition is smooth without intervention |

## Decision Log: Economy

| Decision ID | Scope | Decision | Alternatives | Rationale | Evidence |
| --- | --- | --- | --- | --- | --- |
| DEC-ECO-001 | Basic-security model | Universal Basic Services (UBS) as primary model; cash dividend as secondary supplement | Pure UBI, income-tested welfare, pure UBS | UBS directly guarantees specific welfare outcomes. Universal design builds political coalitions. Cash dividend may supplement for individual choice at margins. | CLM-022, CLM-028, BCM-005 |
| DEC-ECO-002 | Default enterprise form | Cooperative and stakeholder-governed as preferred model; conventional firms permitted with progressive taxation above size thresholds | Mandatory cooperatives, purely conventional, purely public | Worker ownership aligns incentives, reduces inequality, and stabilizes employment. Permission of conventional firms enables entrepreneurial flexibility. Progressive tax nudges toward cooperative form. | BCM-007, CLM-002 |
| DEC-ECO-003 | Care economy | Formal recognition, public support infrastructure, care credits in social security | Market-based care, family-only care, full-state provision | Care work is essential infrastructure (VAL-017). Market-based care creates access inequality. Family-only care creates gender inequality and caregiver burnout. Public support with family choice balances values. | SRC-019, CLM-009 |
| DEC-ECO-004 | Tax architecture | Progressive mix: LVT, income, wealth, ecological, inheritance taxes | Flat tax, consumption-only tax, pure Georgist tax, current OECD-mix status quo | Tax mix internalizes externalities (ecological), reduces concentration (wealth/inheritance), captures socially created value (LVT), and maintains progressivity (income). | SRC-062, SRC-008, CLM-004 |
| DEC-ECO-005 | Automation response | Proactive: reskilling, reduced work hours, automation dividend, job guarantee | Laissez-faire, automation prohibition, full UBI transition | Proactive smoothes transition and distributes gains. Laissez-faire produces concentrated gains with diffused costs. Prohibition inhibits innovation. | SRC-075, SRC-064 |
| DEC-ECO-006 | Central-bank mandate | Multi-mandate: price stability + employment + financial stability + ecological risk | Price stability only, or price stability + employment only | Post-2008 consensus that price stability alone is insufficient. Ecological risk is a financial-stability risk. | SRC-008, SRC-077 |

## Cross-Module Interfaces

| Interface | Partner Module | Coordination Requirement |
| --- | --- | --- |
| Governance | MOD-GOV | Tax authority, fiscal policy, central bank governance, commons governance |
| Ecology | MOD-ECOINF | Ecological accounting, circular economy, land-value assessment, resource taxes |
| Technology | MOD-TAI | Automation tax/policy, data taxation, digital infrastructure as commons |
| Health | MOD-HMH | Healthcare funding, care-economy integration, food-as-health |
| Education | MOD-EDU | Education funding, reskilling entitlement, lifelong learning funding |
| Community | MOD-CUL | Cooperative ecosystem, community care networks, community currencies |
| Defense | MOD-DEF | Strategic autonomy, defense-economy interface, sanctions economics |
| Simulation | MOD-SIM | Model parameters for economic system, tax-incidence modeling |

## Unresolved Questions

- RQ-ECO-001: Commons-layer boundary: where does universal service end and market provision begin? (Architecture proposes specific boundary; simulation should test alternative boundaries.)
- RQ-ECO-004 (from module): Poverty-trap prevention efficacy.
- UBS vs. UBI vs. hybrid: Simulation should compare outcomes across provisioning models.
- Optimal tax rates: Economic modeling required. Architecture proposes progressive structure; exact rates are illustrative and require simulation calibration.
- International trade and capital mobility: This architecture assumes substantial national policy autonomy. Interdependence challenges require MOD-DEF coordination.