# ART-011: Law and Justice System Architecture

Iteration: `baseline-v0.1`
Status: draft

## Purpose

Define the legal order, rights protections, public safety, and justice mechanisms for a legitimate society. The system must protect rights, prevent abuse, provide accessible dispute resolution, and enable member observability of public legal processes while protecting private data.

## Core Design Principles

1. **Law must be public, prospective, consistent, and accessible**: No secret laws. No ex post facto criminal laws. Legal texts and decisions in plain language with translation.
2. **Due process is non-negotiable**: Notice, hearing, counsel, impartial decision-maker, appeal, proportionality.
3. **Multiple justice pathways**: Restorative, rehabilitative, protective, and punitive -- matched to offense type, harm, and context, not ideology.
4. **No one is above the law**: Equal application to citizens, officials, institutions, and foreign actors under jurisdiction.
5. **Rights are enforceable**: Rights without remedies are aspirations. Every right must have at least one accessible enforcement mechanism.
6. **Law must be observable**: Court proceedings, decisions, enforcement actions, and corrections data must be publicly accessible, with privacy protections for victims, minors, and those not convicted.

## Constitutional Rights and Civil Liberties

### Non-Derogable Rights (INESC-001 through INESC-005)

These rights may not be suspended, limited, or derogated under any circumstance, including declared emergencies:

| ID | Right | Definition |
| --- | --- | --- |
| INESC-001 | Freedom from torture | No person shall be subjected to torture or to cruel, inhuman, or degrading treatment or punishment. |
| INESC-002 | Freedom from extrajudicial killing | No person shall be arbitrarily deprived of life by state agents or with state complicity. |
| INESC-003 | Freedom from slavery and forced labor | No person shall be held in slavery or servitude. Forced or compulsory labor is prohibited. |
| INESC-004 | Freedom from forced disappearance | No person shall be subjected to forced disappearance by state agents. |
| INESC-005 | Recognition as a person before the law | Every person has the right to recognition everywhere as a person before the law. |

### Derogable but Strongly Protected Rights (INESC-006 through INESC-020)

These rights may be subject to proportionate limitation during declared emergencies (per DEC-GOV-004 emergency-powers architecture), with mandatory judicial review:

| ID | Right | Definition |
| --- | --- | --- |
| INESC-006 | Right to life and physical security | Protection from arbitrary deprivation of life and from violence. |
| INESC-007 | Liberty and security of person | Freedom from arbitrary arrest, detention, or exile. |
| INESC-008 | Due process and fair trial | Right to a fair and public hearing by an independent and impartial tribunal. |
| INESC-009 | Presumption of innocence | Presumed innocent until proved guilty according to law. |
| INESC-010 | Freedom of thought, conscience, and religion | Including freedom to change religion or belief and to manifest belief in teaching, practice, worship, and observance. |
| INESC-011 | Freedom of expression | Including freedom to seek, receive, and impart information and ideas through any media. |
| INESC-012 | Freedom of peaceful assembly and association | Including the right to form and join trade unions. |
| INESC-013 | Freedom of movement | Right to move freely within the country, to leave any country, and to return to one's country. |
| INESC-014 | Privacy | Protection from arbitrary interference with privacy, family, home, or correspondence. |
| INESC-015 | Right to remedy | Effective remedy by competent tribunals for acts violating fundamental rights. |
| INESC-016 | Equality before the law | Equal protection without discrimination on any ground. |
| INESC-017 | Rights of the child | Special protection and care, including the right to identity, family, and protection from exploitation. |
| INESC-018 | Right to participate in government | Including the right to vote and to stand for election. |
| INESC-019 | Rights of minorities | Persons belonging to minorities shall not be denied the right to enjoy their own culture, profess and practice their own religion, or use their own language. |
| INESC-020 | Data rights | Access to, correction of, deletion of, and portability of personal data; freedom from automated decisions with legal or similarly significant effects without human review. |

### Emergency Limitations

During declared emergencies, derogable rights may be limited subject to:
1. **Legality**: Limitation must be authorized by law, not executive decree alone.
2. **Necessity**: Limitation must be strictly required by the exigencies of the situation.
3. **Proportionality**: Limitation must be the least restrictive means available.
4. **Non-discrimination**: Limitation must not discriminate solely on grounds of race, religion, ethnicity, political opinion, or other protected characteristics.
5. **Judicial review**: Every limitation must be reviewable by an independent court within 7 days.
6. **Duration**: Limitations expire with emergency declaration unless reauthorized.
7. **Notification**: International notification obligations must be fulfilled.

**Decision**: DEC-LAW-001 (non-derogable-rights list). Rationale: International human-rights law consensus identifies torture, extrajudicial killing, slavery, and forced disappearance as non-derogable. Additional non-derogable rights beyond international minimum are debated but this architecture adopts the consensus floor. Future iteration may expand.

## Court System Architecture

### Tiers

1. **Community Justice Circles**: First-instance resolution for minor disputes, neighborhood conflicts, community-norm violations. Facilitated by trained community mediators. Voluntary except where mandated as diversion from formal system. Decisions may be appealed to Community Court.

2. **Community Courts**: First-instance formal court for misdemeanors, small civil claims (<threshold), family law, and community-constitution questions. Single judge or 3-judge panel. Located within clusters of community cells (accessible within 30 minutes travel).

3. **Regional Courts**: First-instance for felonies, civil claims above threshold, administrative law, and appeals from Community Courts. Also constitutional questions within regional jurisdiction. 3-judge panels. Jury option for serious criminal cases.

4. **Regional Courts of Appeal**: Appellate review of Regional Court decisions. 5-judge panels. Review for errors of law, procedure, and manifestly unreasonable factual findings. No de novo trial.

5. **Constitutional Court**: Final appellate jurisdiction for constitutional questions, fundamental-rights violations, and inter-tier governance disputes. 9 judges (DEC-GOV-003). Constitutional review of legislation before and after enactment.

6. **Specialized Tribunals**: Environmental Court, Technology and Data Court, Anti-Corruption Tribunal, Labor Court, Family Court -- with specialized judges and procedures. Appeals to Regional Courts of Appeal and Constitutional Court on constitutional questions.

### Judicial Independence and Selection

- **Judicial Nominations Commission (JNC)**: Independent body comprising judges, legal academics, citizen representatives (sortition), and practicing lawyers. Prepares shortlists of qualified candidates for judicial appointments. Composition resists political capture through mixed membership and staggered terms.

- **Selection**: Judges appointed from JNC shortlists by confirmation vote (2/3 majority for Constitutional Court, simple majority for others by relevant assembly).

- **Tenure**: Constitutional Court: 15-year non-renewable terms. Other appellate: 12-year non-renewable. Trial courts: 10-year renewable once.

- **Removal**: Only for incapacity, gross misconduct, or conviction of serious crime. Removal by 2/3 vote of Constitutional Court (for Constitutional Court judges) or Judicial Conduct Commission.

- **Budget**: Judicial budget indexed to population and caseload; not subject to annual political negotiation.

- **Prosecutorial Independence**: Prosecutors organized as independent service, headed by Director of Public Prosecutions appointed by JNC for 10-year non-renewable term. Prosecutorial decisions insulated from political direction.

**Decision**: DEC-LAW-002 (judicial-appointment model). Rationale: Joint JNC + confirmation model balances expertise (JNC shortlisting) with democratic legitimacy (assembly confirmation). Non-renewable long terms prevent reappointment incentives to curry favor. Indexed budget prevents financial pressure.

---

## Public Safety Architecture

### Policing Design Principles

1. **Public safety, not force projection**: Police are community safety partners, not an occupying force.
2. **Procedural justice**: Every interaction should be governed by respect, neutrality, voice (opportunity to be heard), and trustworthiness.
3. **Accountability**: Every use of force is reported, reviewed, and published in aggregated form.
4. **Minimum necessary force**: Force continuum with de-escalation as default.
5. **Community integration**: Police live in communities they serve. Community oversight boards with real authority.

### Policing Structure

- **Community Safety Officers**: Unarmed, community-embedded. Primary role: presence, relationship-building, conflict de-escalation, vulnerability identification, emergency first response. Selected from community where feasible.
- **Police Officers**: Armed, trained in de-escalation, crisis intervention, and procedural justice. Respond to incidents requiring enforcement capacity. Minimum 2-year training program including community placement.
- **Specialist Units**: Investigation, forensics, organized crime, cybercrime, counter-terrorism. Separate from community policing.
- **Independent Police Oversight Authority**: Civilian body with investigative power, subpoena authority, and disciplinary recommendation power. Membership includes civil-liberties, community, and legal representatives. Investigates all deaths in custody, serious injuries, firearms discharges, and complaints of excessive force or discrimination.

### Use-of-Force Architecture
- **Continuum**: Presence > Verbal > Soft empty-hand > Hard empty-hand > Less-lethal weapons > Lethal force.
- **Reporting**: Every use of force above verbal reported within 24 hours. Lethal force and serious injury investigated by Independent Oversight Authority.
- **Data**: Use-of-force data published quarterly, disaggregated by officer, location, demographic, and outcome.
- **Body cameras**: Mandatory and tamper-proof. Footage retained, auditable, accessible to subjects and oversight.
- **Duty to intervene**: Officers have legal duty to intervene when witnessing excessive force by colleagues. Failure to intervene is a criminal offense.

**Decision**: DEC-LAW-003 (public-safety architecture). Rationale: Community-safety model with unarmed community officers + armed specialists parallels successful models in Scotland, Norway, New Zealand, and other jurisdictions with lower police-violence rates. Procedural-justice emphasis (BF-003, BF-010) directly addresses trust and legitimacy.

---

## Justice Pathways

The system offers multiple justice pathways, matched to offense type, harm severity, victim preference, and offender circumstances:

### Pathway 1: Restorative Justice
- **Scope**: Non-violent offenses, youth offenses, first-time offenses, community-level conflicts, victim-requested cases.
- **Process**: Facilitated dialogue between harmed and responsible parties. Outcome agreement: apology, restitution, community service, behavioral commitments. Monitored for compliance.
- **Effect**: Successful completion may expunge record. Failure may escalate to Pathway 2 or 3.
- **Evidence**: Restorative justice reduces recidivism ~10-30% vs. punitive approaches for eligible offenses (moderate confidence -- meta-analytic evidence).

### Pathway 2: Rehabilitative Justice
- **Scope**: Offenses related to addiction, mental health, trauma, or social circumstances where treatment and support have higher social return than punishment.
- **Process**: Assessment by multidisciplinary team (legal, clinical, social work). Individualized rehabilitation plan with treatment, education, community service, victim restitution. Court-supervised with progress reviews.
- **Effect**: Successful completion may reduce sentence or expunge record. Non-compliance escalates to Pathway 3.

### Pathway 3: Protective and Punitive Justice
- **Scope**: Violent offenses, repeat offenses, offenses where community protection requires incapacitation, or where victim and community interest require punitive response.
- **Process**: Traditional criminal trial with all due-process protections. Sentencing guided by proportionality, public safety, rehabilitation possibility, and victim impact.
- **Sentencing principles**:
  - Incarceration as last resort, not default.
  - Maximum sentence lengths specified, not open-ended.
  - Mandatory rehabilitation programming during incarceration.
  - Post-release support mandatory (housing, employment, healthcare, community transition).
  - Death penalty prohibited.
  - Solitary confinement limited to 15 days maximum, with judicial review.
  - Juvenile justice entirely separate with emphasis on rehabilitation.

### Pathway 4: Community Separation (for reform-resistant violent offenders)
- **Scope**: High-risk violent offenders where rehabilitation repeatedly failed and community protection requires long-term separation.
- **Process**: Separate review board (legal, clinical, community) determines necessity. Annual review. Treatment and humane conditions maintained. This is protective, not punitive in intent.
- **Safeguards**: Appeal to Constitutional Court. Maximum 5-year orders renewable only with new evidence. Not punitive punishment; conditions must meet or exceed general living standards.

**Decision**: DEC-LAW-004 (multi-pathway justice). Rationale: Single-pathway punitive justice produces high recidivism, massive fiscal cost, and intergenerational harm without commensurate public-safety benefit. Multi-pathway system tailors response to context. Restorative and rehabilitative approaches have better outcomes for eligible cases (moderate confidence). Protective separation reserved for cases where community safety requires it.

---

## Legal-Access Architecture

### Right to Counsel
- Universal civil and criminal legal aid, free at point of use.
- Public defender service: competitive salary, manageable caseload caps, independence from prosecution.
- Community legal clinics: embedded in community cells, providing basic legal advice, triage, and referral.
- Legal self-help tools: publicly maintained, professionally reviewed, in plain language and multiple languages.

### Alternative Dispute Resolution
- **Community mediation**: First-resort for non-criminal disputes. Trained community mediators. Low-cost, fast, relationship-preserving.
- **Ombuds institutions**: Sector-specific ombuds (healthcare, education, government services, financial, housing, technology) with investigatory and recommendation powers.
- **Restorative conferencing**: For appropriate criminal, school, workplace, and community cases.

### Legal Observability
- All court decisions published (with victim, minor, and privacy redactions).
- Sentencing data publicly available: by offense type, by judge, by demographic (to detect disparity).
- Court performance metrics: case-processing time, trial-to-resolution ratio, appeal rate, reversal rate.
- Prosecution data: charging decisions, plea offers, dismissals -- by offense and demographic.
- Police data: stops, searches, arrests, use of force -- by location, demographic, and outcome.
- Corrections data: population, demographics, conditions, incidents, rehabilitation participation, recidivism.
- All data publicly accessible but subject to privacy protections for individuals.

**Decision**: DEC-LAW-005 (legal observability). Rationale: Legal-system opacity enables discrimination, corruption, and institutional decay. Comprehensive observability aligned with VAL-019. Privacy protections prevent weaponization of data against individuals.

---

## Detention and Corrections Architecture

### Principles
1. **Deprivation of liberty is the punishment, not deprivation of dignity, safety, or health**.
2. **Incarceration must not create additional harm**: violence, trauma, disease, family destruction, employability destruction.
3. **Rehabilitation is the primary institutional goal of incarceration**.
4. **Reentry begins on day one of sentence**.

### Design Requirements
- **Small facilities**: Maximum 200-person facilities, organized as therapeutic communities. No mega-prisons.
- **Normalization principle**: Living conditions approximate community norms (own clothing, personal space, cooking facilities, meaningful activity).
- **Family connection**: Generous visitation (in-person, video), family-therapy integration, parenting programs. Facilities located near population centers.
- **Healthcare and mental healthcare**: Equivalent to community standard, not inferior.
- **Education and work**: Education programs, vocational training, meaningful work with marketable skills, fair compensation.
- **Transition support**: Pre-release planning, housing placement, employment placement, healthcare continuity, community supervision (supportive, not purely surveillance).
- **Voting rights**: Voting rights restored upon sentence completion. No permanent disenfranchisement.
- **Private prisons prohibited**: All detention and corrections publicly operated, publicly accountable.

---

## Evidence and Assumptions

### Key Evidence Claims Used

| Claim ID | Application |
| --- | --- |
| CLM-029 | Judicial independence reduces corruption and protects rights. |
| CLM-016 | Trauma-informed institutional design improves justice outcomes. |
| CLM-031 | Transparency must be paired with enforcement to reduce corruption. |
| CLM-009 | ACEs predict criminal-justice involvement; prevention is cost-effective. |

### Key Assumptions

| Assumption ID | Statement | Test Method | Failure Signal |
| --- | --- | --- | --- |
| ASM-LAW-001 | Restorative justice reduces recidivism for eligible offenses compared to punitive responses | Randomized controlled trials; longitudinal recidivism tracking | Reconviction rate equal or higher in restorative pathway |
| ASM-LAW-002 | Community-safety-officer model reduces use of force and improves police-community trust | Pilot implementation with comparison communities; force-reporting data; trust surveys | No significant reduction in force or trust improvement vs. traditional model |
| ASM-LAW-003 | Legal observability identifies and deters discrimination without producing perverse incentives | Data analysis of observability effects in existing transparency jurisdictions | Gaming of metrics detected; discrimination not reduced despite transparency |

## Decision Log: Law and Justice

| Decision ID | Scope | Decision | Alternatives | Rationale | Evidence |
| --- | --- | --- | --- | --- | --- |
| DEC-LAW-001 | Non-derogable rights | 5 non-derogable rights (torture, extrajudicial killing, slavery, forced disappearance, recognition as person) | No non-derogable rights, broader list | International legal consensus on core non-derogable rights. Broader list faces enforcement credibility problem. | SRC-001, SRC-045, international human-rights instruments |
| DEC-LAW-002 | Judicial appointments | JNC shortlists + assembly confirmation; non-renewable long terms; indexed budget | Direct election of judges, pure executive appointment, career judiciary | Balances expertise (JNC), democratic legitimacy (confirmation), and independence (non-renewable terms + indexed budget). | SRC-010, CLM-029 |
| DEC-LAW-003 | Public safety | Community Safety Officers (unarmed) + Police (armed) + Independent Oversight Authority | Traditional armed police only, fully unarmed police | Evidence from lower-violence jurisdictions shows community-embedded, procedure-justice-oriented policing reduces force and improves trust. Unarmed primary responders de-escalate and triage. | SRC-018 (mental-health crisis response evidence) |
| DEC-LAW-004 | Justice pathways | 4 pathways: restorative, rehabilitative, punitive/protective, community separation | Single punitive-only pathway, restorative-only pathway | Tailored response to different offense and offender types. Restorative for eligible cases reduces recidivism. Punitive retained for serious and repeat offenses. Community separation as last resort. | Meta-analytic evidence on restorative justice; Nordic rehabilitative model (BCM-005) |
| DEC-LAW-005 | Legal observability | Comprehensive public data on all legal-system operations with individual privacy protections | Limited public data, opaque system | VAL-019 requires observability of public processes. CLM-031 shows transparency + enforcement reduces corruption. Privacy protections prevent individual harm. | SRC-034, SRC-011 |

## Cross-Module Interfaces

| Interface | Partner Module | Coordination Requirement |
| --- | --- | --- |
| Governance | MOD-GOV | Constitutional Court jurisdiction; emergency-powers legal limits; governance accountability mechanisms; observability legal framework |
| Health | MOD-HMH | Mental-health-court integration; addiction treatment vs. criminalization; trauma-informed justice |
| Community | MOD-CUL | Community mediation; restorative justice at community level; community-reintegration support |
| Technology | MOD-TAI | Algorithmic decision limits in justice; digital evidence rules; cybersecurity of justice systems; AI in legal aid |
| Defense | MOD-DEF | Military justice; emergency-powers interface; intelligence oversight |
| Education | MOD-EDU | Juvenile justice; school-discipline reform; civic legal education |

## Unresolved Questions

- RQ-LAW-001: Non-derogable-rights list -- should it be expanded beyond international-consensus floor? Future iteration to evaluate.
- RQ-LAW-003: Community-separation criteria require more detailed specification and testing.
- RQ-LAW-004: Restorative vs. punitive balance in specific offense categories requires ongoing data collection and adjustment.
- RQ-LAW-006: Detailed observability-rights legal framework needs MOD-TAI coordination for technical implementation.