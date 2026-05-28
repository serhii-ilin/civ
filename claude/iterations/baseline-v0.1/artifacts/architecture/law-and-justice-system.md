# Law and Justice System

Artifact ID: ART-011
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: MOD-LAW
Depends on: ART-008, ART-009

## Purpose

Specify the legal order: which rights are protected and how, how laws are made and accessed, how courts and prosecution are organized, how public safety is delivered without abuse, how restorative and rehabilitative pathways are constructed, and how the system corrects itself. Bound by `value-constitution.md` (ART-008) and the governance design in ART-009.

The central principles are: rights protect persons against state and concentrated private power, due process is non-derogable, law is accessible in language and cost, force is the last resort, and the system tracks and corrects its own errors.

## Sources of Law (LAW-S)

### LAW-S1 Constitution

- The constitution (synthesizing `value-constitution.md` and the governance architecture) is the supreme law.
- Constitutional Court (GOV-B3) has the final word on constitutional interpretation.

### LAW-S2 Statutes

- Acts of the Representative Assembly (GOV-B2), where applicable confirmed by Sortition Chamber (GOV-B6).
- Publicly available in machine- and human-readable form within 7 days of enactment.

### LAW-S3 Regulations

- Made by Executive Council departments (GOV-B4) and independent regulators (GOV-B10) under statutory authority.
- Subject to public consultation, impact assessment, sunset clauses (default 7 years), and judicial review for ultra vires action.

### LAW-S4 Case Law

- Decisions of higher courts have binding precedent on lower courts within their jurisdiction.
- Courts disclose reasoning; dissents are published.

### LAW-S5 Customary Law

- Recognized within constitutional limits; particularly relevant for indigenous communities and pre-existing community jurisdictions.
- Customary law cannot override universal rights (TZ-002, TZ-006).

### LAW-S6 International Law

- Ratified treaties incorporated per GOV-D4.
- Customary international law and jus cogens norms applied where consistent with constitutional rights.

## Rights and Protections (LAW-R)

### LAW-R1 Civil and Political Rights

Enumerated and judicially enforceable. Includes (non-exhaustively):

- Life, bodily integrity, and security of person.
- Freedom from torture, cruel, inhuman, or degrading treatment.
- Freedom from arbitrary detention.
- Freedom of conscience, religion, and belief.
- Freedom of expression and protected speech, including dissent, satire, and journalism.
- Freedom of association and peaceful assembly.
- Freedom of movement and residence within the polity.
- Privacy, including informational and bodily privacy.
- Due process: notice of charges, fair hearing, defense counsel, presumption of innocence, prohibition on self-incrimination, public trial, appeal, prohibition on double jeopardy, prohibition on ex post facto laws.
- Equal protection under law; non-discrimination.
- Right to legal personality; right to a nationality.
- Voting rights for citizens; political participation.
- Access to information held by public bodies (subject to narrow exceptions).

### LAW-R2 Economic, Social, and Cultural Rights

Enumerated and progressively realizable, with judicial enforcement of core minima.

- Education (LAW-R2.1).
- Healthcare, including mental health (LAW-R2.2).
- Adequate housing (LAW-R2.3).
- Food and water security (LAW-R2.4).
- Work and just conditions of work (LAW-R2.5).
- Social security and care (LAW-R2.6).
- Cultural participation and minority cultural rights (LAW-R2.7).
- A healthy environment (LAW-R2.8).

### LAW-R3 Group and Collective Rights

- Indigenous peoples' rights, including land, language, and self-governance within constitutional limits.
- Minority rights to language, education, and cultural institutions.
- Rights of children: best-interest standard, participation rights, protection.
- Rights of disabled members: accessibility, accommodation, participation.

### LAW-R4 Digital and Algorithmic Rights

- Right to access one's own personal data held by any body.
- Right to explanation for high-impact algorithmic decisions.
- Right to human review of high-impact algorithmic decisions.
- Right to non-deception (regulated against deceptive design patterns).
- See ART-016.

### LAW-R5 Non-Derogable Core (Even in Emergency)

- Right to life (subject to lawful self-defense and use-of-force rules).
- Freedom from torture and cruel treatment.
- Freedom from slavery.
- Freedom of conscience.
- Recognition before law.
- Prohibition on retroactive criminal liability.
- Right to non-discrimination on prohibited grounds.

### LAW-R6 Standing and Remedy

- Members have standing to enforce their rights through courts.
- Civil society and ombuds bodies have third-party standing in defined cases.
- Constitutional Court can issue declarations of incompatibility against legislation; Representative Assembly must respond within 12 months.
- Damages, injunctive relief, declaratory relief, and structural remedies available.

## Courts and Tribunals (LAW-C)

### LAW-C1 Court Hierarchy

- Constitutional Court (GOV-B3): constitutional matters, inter-body conflicts, election disputes, declarations of incompatibility.
- Supreme Court: final appellate court for civil and criminal matters.
- Regional Courts of Appeal.
- Trial Courts at local and regional level.
- Specialized Tribunals: administrative, labor, family, juvenile, tax, asylum, intellectual property, environmental.
- Customary or Community Courts: where established by community charter and consistent with constitutional rights.

### LAW-C2 Judicial Independence

- Tenure protection (single 12-year term for Constitutional Court; 15-year term for other senior judges; renewable in specific cases through reappointment by mixed bodies).
- Salaries set by independent commission; cannot be reduced during tenure.
- Public reasoning required; dissents published.
- Conflicts of interest declared.
- Removal only for cause through specified procedure (GOV-R).

### LAW-C3 Judicial Selection

- Mixed nomination per GOV-S3.
- Diversity of background actively pursued (legal, professional, demographic).
- Qualification assessment with transparent rubrics.

### LAW-C4 Access to Justice

- Legal aid for all serious criminal matters and substantial civil matters where rights are at stake.
- Simplified procedures and self-help support for small-claims and family matters.
- Translation and interpretation services.
- Online filing and case-tracking with universal physical fallback for digital-excluded members.
- Court fees structured to be progressive; fee waivers for indigent parties.

### LAW-C5 Alternative Dispute Resolution

- Mediation, restorative conferencing, arbitration available with protections against coercion.
- ADR cannot override fundamental rights protections.
- ADR processes recorded for accountability.

## Prosecution and Police (LAW-P)

### LAW-P1 Prosecution

- Public prosecution service operationally independent of the executive.
- Prosecutor General appointed for non-renewable 8-year term by mixed bodies; protected against dismissal except for cause.
- Prosecutorial guidelines public; major decisions documented.
- Prosecutor decisions not to charge subject to judicial review in specified categories.
- Specialized units for corruption, organized crime, hate crime, environmental crime, financial crime, AI-related crime.

### LAW-P2 Public Safety Services

- Multi-modal model: civilian first responders for non-violent calls (mental health crisis teams, social workers, mediators); trained police officers for violent or armed incidents; community safety partners for prevention and presence.
- Civilian oversight body at each operational level with subpoena and discipline powers.
- Use-of-force policies: proportionality, de-escalation as default, lethal force only when necessary to prevent death or grievous harm.
- Body cameras and incident recording required; tampering is a serious offense.
- Pattern-or-practice review by GOV-B5 when complaints exceed threshold.

### LAW-P3 Police Selection and Training

- Selection criteria explicitly screen against authoritarian personality markers and unaddressed trauma; psychological assessment and ongoing support.
- Training duration substantially longer than current minimums in many jurisdictions; includes de-escalation, mental-health crisis response, cultural literacy, constitutional rights.
- Continuing education and recertification required.

### LAW-P4 Investigation and Surveillance Powers

- Search and seizure require judicial warrant on probable cause for most categories.
- Surveillance (electronic, location, communications) requires warrant with specific factual basis; warrant duration limited; mandatory disclosure after operation closes.
- Mass surveillance prohibited; targeted surveillance only.
- See ART-016 for digital-investigation specifics.

### LAW-P5 Detention

- Pre-trial detention is the exception, not the rule; risk-based and reviewed within 48 hours.
- Detention conditions audited; standards consistent with international law on detention.
- Limits on solitary confinement; prohibition on punitive isolation of children and detainees with mental illness.
- Independent inspector general for detention facilities.

### LAW-P6 Border and Immigration Enforcement

- Bound by constitutional rights of non-citizens at border, asylum-seekers, refugees, and immigrants (LAW-R5 non-derogable applies to all persons under jurisdiction).
- Detention of asylum-seekers limited; alternatives to detention preferred.
- See ART-017.

## Criminal Justice (LAW-CJ)

### LAW-CJ1 Substantive Criminal Law

- Crimes are defined narrowly, in statute, with clear elements.
- Mens rea required for serious crimes; strict liability limited.
- Disproportionate sentencing prohibited (constitutional review).
- No criminalization of status (homelessness, addiction, identity).

### LAW-CJ2 Procedural Protections

- All LAW-R1 due-process protections; counsel of choice or appointed; right to remain silent; protection against coerced confession; speedy trial.
- Discovery obligations on prosecution.
- Jury trial right for serious offenses, with jury selection processes transparent and bias-tested.

### LAW-CJ3 Restorative and Rehabilitative Justice

- Restorative pathways available for many offenses where victim, offender, and community consent (CLM-091).
- Diversion programs for first-time and lower-severity offenses, particularly for young people and people with mental health or substance-use issues.
- Probation, supervised release, community service as alternatives to incarceration where consistent with public safety.

### LAW-CJ4 Incarceration

- Reserved for offenses where separation from community is necessary for public safety, deterrence is plausibly required, or restorative pathways have failed.
- Facility conditions: humane standards; education, healthcare, mental healthcare, vocational training available; visits and family contact protected.
- Sentence length capped at proportional ceilings; whole-life sentences only in extreme cases with constitutional review.

### LAW-CJ5 Reentry

- Pre-release planning; housing, employment support, healthcare continuity.
- Restoration of civil rights (including voting) post-sentence by default, not by petition.
- Sealing or expungement of records for non-violent offenses after defined period.

### LAW-CJ6 Specialized Offenses

- Corruption: aggressive prosecution; mandatory forfeiture of proceeds; long ineligibility for office.
- Hate crime: enhanced penalties; victim-support services; community-level response.
- Domestic and sexual violence: trauma-informed investigation; victim-centered procedures; specialist courts.
- Financial crime: serious treatment of large-scale fraud, tax evasion, money laundering.
- Environmental crime: ecocide as recognized offense; restitution to ecological commons.
- AI- and algorithm-related crime: see ART-016.

## Civil Law (LAW-CV)

### LAW-CV1 Contract and Tort

- Standard private-law framework with consumer-protection and unequal-bargaining-power doctrines.
- Class actions and collective redress available for mass harms.

### LAW-CV2 Family Law

- Marriage and partnership recognition open without discrimination on protected grounds.
- Child welfare with best-interest standard, child participation rights, due process for parents.
- Divorce and dissolution with no-fault grounds.
- Adoption with rights-respecting procedures.

### LAW-CV3 Property Law

- Standard property law subject to ECO-L5 (land), ECO-P3 (housing), ECO-P4 (intellectual property).
- Eminent domain or compulsory purchase available for public purpose with fair compensation and public-interest review.

### LAW-CV4 Employment Law

- Worker protection, anti-discrimination, collective rights per ECO-W.
- Employment tribunals with simplified procedures.

### LAW-CV5 Public-Interest Standing

- Civil society organizations and ombuds bodies have standing in defined categories to sue on behalf of affected groups.

## Administrative Law (LAW-AD)

- Decisions of public bodies must be reasoned, in writing, and subject to administrative appeal.
- Judicial review for legality, procedural fairness, and rationality.
- Time limits on administrative decisions; deemed-approval where appropriate to prevent paralysis (with safeguards).
- Right to be heard before adverse decisions affecting rights or material interests.

## Anti-Corruption (LAW-AC)

- Dedicated anti-corruption commission as one of GOV-B10 regulators.
- Asset disclosure for senior officials (GOV-A1).
- Whistleblower protection (GOV-A6).
- Specialized prosecution unit.
- Mandatory forfeiture of proceeds of corruption.
- Long ineligibility for office post-conviction.
- Public registry of beneficial ownership of legal entities.

## Emergency Law (LAW-E)

Bound by TZ-001 and GOV-D5:

- Emergency declarations must specify the threat, the powers invoked, the duration, the geographical scope, and the reporting frequency.
- Non-derogable rights (LAW-R5) hold throughout.
- Courts continue to operate; habeas corpus remains available.
- Sunset and renewal procedures (GOV-D5) bind.

## Member Observability and Privacy (LAW-O)

- Court hearings are public by default; closed hearings require specific cause (national security, child welfare, witness protection) and are documented as closed.
- Decisions and reasoning are published with appropriate redactions; redaction criteria are public.
- Statistics on cases, sentences, complaints, and outcomes are published in aggregate.
- Personal data of parties, victims, witnesses is protected; reporters' shield laws balance press access against privacy.
- See VAL-019 and TZ-004.

## Indicators (LAW-I)

- Rights violations: complaints, findings, remedies, time to resolution.
- Due process: case-duration distributions, success on appeal, wrongful conviction findings.
- Prosecutorial: case selection patterns, conviction rates by category, disparity audits.
- Police: use-of-force frequency, complaints, sustained complaints, officer mental-health, community trust.
- Detention: population, conditions audit results, mental healthcare access, deaths in custody.
- Civil access: legal-aid coverage, fee-waiver rates, case-resolution times in family and small-claims courts.
- Restorative: program availability, participation, victim and offender satisfaction, reoffending outcomes.
- Re-entry: post-release housing, employment, mental healthcare continuity, civil rights restoration.

Disparity audits run regularly: do outcomes differ by race, gender, region, disability, language at statistically significant levels after controlling for offense severity and prior record? Findings drive structural review by GOV-B5.

## Open Issues

- Restorative-justice evidence is mixed (CLM-091); the framework's reliance on it requires careful program-design and ongoing measurement.
- The boundary between speech protection and harm regulation (defamation, harassment, incitement) is contested; the framework adopts a narrow harm test and judicial review.
- Plea bargaining is recognized as both efficient and coercive; the framework restricts it with judicial supervision and victim consultation.
- Customary-law-versus-constitutional-rights conflicts (LAW-S5) require case-by-case resolution; the framework hedges by retaining ultimate constitutional review.
- AI-related crime (deepfakes, automated fraud, algorithmic discrimination) is under-elaborated here; see ART-016 for technical detail.
- Climate-related rights enforcement (LAW-R2.8) is novel; emerging case law in various jurisdictions provides early guidance only.

## Cross-References

- Bound by: VAL-001, VAL-005, VAL-008, VAL-010, VAL-015, VAL-019.
- Coordinates with: ART-009 (governance), ART-016 (technology), ART-017 (defense), ART-014 (community), ART-012 (health for mental-health-related criminal cases).
- Tested in: stress scenarios on judicial pressure, surveillance creep, emergency-power ratchet, mass-protest policing, due-process under crisis.
