# Source Register

Artifact ID: ART-003
Iteration: baseline-v0.1
Status: draft
Change type: new
Owner module: MOD-RES

## Purpose

Registry of external sources used by claims (CLM-*), benchmarks, failure modes, and behavioral foundations in this iteration. Citations are conservative: well-known works and standing datasets. Where exact metadata (DOI, page range) was not verified at write time, the `URL/DOI` field is marked `unverified` and must be resolved before this artifact moves from `draft` to `reviewed`.

Reliability notes record known caveats: contested claims, replication failures, ideological framing, dataset gaps, or selection bias in the source itself.

## Source Table

| Source ID | Citation | URL/DOI | Type | Used In | Reliability Notes |
| --- | --- | --- | --- | --- | --- |
| SRC-001 | Tainter, Joseph A. (1988). *The Collapse of Complex Societies*. Cambridge University Press. | ISBN 978-0521386739 | Book / historical synthesis | CLM-001, CLM-002, CLM-030 | Influential but mono-causal (declining marginal returns on complexity); pair with multi-cause works. |
| SRC-002 | Acemoglu, D., & Robinson, J. A. (2012). *Why Nations Fail*. Crown. | ISBN 978-0307719218 | Book / political economy | CLM-003, CLM-004, CLM-060 | "Inclusive vs. extractive" frame is useful but criticized for circular definition; treat as one lens. |
| SRC-003 | Acemoglu, D., & Robinson, J. A. (2019). *The Narrow Corridor*. Penguin. | ISBN 978-0735224384 | Book / political theory | CLM-005, CLM-061 | Continuation of SRC-002; cites historical cases selectively. |
| SRC-004 | Scheidel, W. (2017). *The Great Leveler*. Princeton University Press. | ISBN 978-0691165028 | Book / historical economics | CLM-006, CLM-070 | Thesis (inequality only falls after catastrophe) is contested. |
| SRC-005 | Turchin, P. (2016). *Ages of Discord*. Beresta Books. | ISBN 978-0996139540 | Book / cliodynamics | CLM-007, CLM-031 | Quantitative-historical; predictive claims not all validated. |
| SRC-006 | Ostrom, E. (1990). *Governing the Commons*. Cambridge University Press. | ISBN 978-0521405997 | Book / institutional economics | CLM-010, CLM-011, CLM-080 | Foundational; design principles widely replicated across commons studies. |
| SRC-007 | Putnam, R. (2000). *Bowling Alone*. Simon & Schuster. | ISBN 978-0743203043 | Book / social capital | CLM-012, CLM-090 | US-centric; some indicators have rebounded or shifted form. |
| SRC-008 | Putnam, R. (1993). *Making Democracy Work*. Princeton University Press. | ISBN 978-0691037387 | Book / comparative politics | CLM-013, CLM-091 | Italian regional study; causal direction (civic culture → institutional performance) contested. |
| SRC-009 | Fukuyama, F. (2011). *The Origins of Political Order*. Farrar, Straus and Giroux. | ISBN 978-0374533229 | Book / political history | CLM-014 | Sweeping synthesis; ideological framing flagged by critics. |
| SRC-010 | Fukuyama, F. (2014). *Political Order and Political Decay*. Farrar, Straus and Giroux. | ISBN 978-0374227357 | Book / political history | CLM-015 | See SRC-009 caveats. |
| SRC-011 | Levitsky, S., & Ziblatt, D. (2018). *How Democracies Die*. Crown. | ISBN 978-1524762933 | Book / comparative politics | CLM-016, CLM-100 | Pattern-matching across cases; selection-biased toward recent backsliding. |
| SRC-012 | Manin, B. (1997). *The Principles of Representative Government*. Cambridge University Press. | ISBN 978-0521458917 | Book / political theory | CLM-017, CLM-101 | Historical-theoretical; light on quantitative evidence. |
| SRC-013 | Landemore, H. (2020). *Open Democracy*. Princeton University Press. | ISBN 978-0691181998 | Book / political theory | CLM-018, CLM-102 | Strong on sortition theory; light on long-horizon evidence. |
| SRC-014 | Piketty, T. (2014). *Capital in the Twenty-First Century*. Belknap Press. | ISBN 978-0674430006 | Book / economics | CLM-020, CLM-110 | Data widely cited; r > g framing contested; underlying WID dataset (SRC-015) is more durable. |
| SRC-015 | World Inequality Database. | wid.world | Dataset | CLM-021, CLM-110 | Methodological choices contested but transparent. |
| SRC-016 | Saez, E., & Zucman, G. (2019). *The Triumph of Injustice*. W. W. Norton. | ISBN 978-1324002727 | Book / public finance | CLM-022 | US-focused; tax-progressivity claims contested by alternative methodologies. |
| SRC-017 | Mazzucato, M. (2013). *The Entrepreneurial State*. Anthem Press. | ISBN 978-0857282521 | Book / industrial policy | CLM-023 | Case-study heavy; counterfactuals weak. |
| SRC-018 | Raworth, K. (2017). *Doughnut Economics*. Chelsea Green. | ISBN 978-1603586740 | Book / heterodox economics | CLM-024, CLM-120 | Framework, not empirical study; useful conceptual scaffold. |
| SRC-019 | Banerjee, A., & Duflo, E. (2019). *Good Economics for Hard Times*. PublicAffairs. | ISBN 978-1610399500 | Book / development economics | CLM-025 | RCT-informed; generalization beyond studied contexts is limited. |
| SRC-020 | Atkinson, A. B. (2015). *Inequality: What Can Be Done?* Harvard University Press. | ISBN 978-0674504769 | Book / public economics | CLM-026 | Policy menu, evidence varies by proposal. |
| SRC-021 | Daly, H., & Farley, J. (2010). *Ecological Economics* (2nd ed.). Island Press. | ISBN 978-1597266819 | Textbook / ecological economics | CLM-027 | Foundational; heterodox framing. |
| SRC-022 | Acemoglu, D., & Restrepo, P. (2020). "Robots and Jobs: Evidence from US Labor Markets." *Journal of Political Economy*, 128(6). | doi.org/10.1086/705716 | Peer-reviewed paper | CLM-028 | Industry-level identification; results vary by labor market. |
| SRC-023 | Marmot, M. (2015). *The Health Gap*. Bloomsbury. | ISBN 978-1408857991 | Book / social determinants of health | CLM-040, CLM-130 | Pairs with Whitehall studies (SRC-024). |
| SRC-024 | Marmot, M. G., et al. Whitehall II Study (ongoing). UCL. | ucl.ac.uk/whitehallII | Longitudinal cohort | CLM-040 | Civil-servant sample; external validity must be argued case by case. |
| SRC-025 | Wilkinson, R., & Pickett, K. (2009). *The Spirit Level*. Allen Lane. | ISBN 978-1846140396 | Book / population health | CLM-041 | Cross-country correlations; causal interpretation contested. |
| SRC-026 | Holt-Lunstad, J., et al. (2015). "Loneliness and Social Isolation as Risk Factors for Mortality." *Perspectives on Psychological Science*, 10(2). | doi.org/10.1177/1745691614568352 | Meta-analysis | CLM-042 | Robust effect size; specific mechanism debated. |
| SRC-027 | Felitti, V. J., et al. (1998). "Adverse Childhood Experiences and Adult Health." *American Journal of Preventive Medicine*, 14(4). | doi.org/10.1016/S0749-3797(98)00017-8 | Cohort study | CLM-043 | Replicated; recall bias and selection caveats apply. |
| SRC-028 | Hattie, J. (2009). *Visible Learning*. Routledge. | ISBN 978-0415476188 | Meta-meta-analysis / education | CLM-050 | Effect-size methodology criticized; use as ordering, not absolute. |
| SRC-029 | Deci, E. L., & Ryan, R. M. (2017). *Self-Determination Theory*. Guilford. | ISBN 978-1462528769 | Book / psychology | CLM-051, CLM-150 | Strong replication record across cultures. |
| SRC-030 | Heckman, J. J. (2006). "Skill Formation and the Economics of Investing in Disadvantaged Children." *Science*, 312(5782). | doi.org/10.1126/science.1128898 | Peer-reviewed paper | CLM-052 | Causal claims about specific programs; generalization debated. |
| SRC-031 | OECD. Programme for International Student Assessment (PISA), most recent cycle. | oecd.org/pisa | Dataset | CLM-053 | Cross-country comparability caveats well documented. |
| SRC-032 | Henrich, J. (2020). *The WEIRDest People in the World*. Farrar, Straus and Giroux. | ISBN 978-0374173227 | Book / cultural evolution | CLM-060, CLM-160 | Macro-historical claims contested; psychometric WEIRD evidence stronger. |
| SRC-033 | Henrich, J. (2015). *The Secret of Our Success*. Princeton University Press. | ISBN 978-0691166858 | Book / cultural evolution | CLM-061 | See SRC-032. |
| SRC-034 | Dunbar, R. I. M. (1992). "Neocortex size as a constraint on group size in primates." *Journal of Human Evolution*, 22(6). | doi.org/10.1016/0047-2484(92)90081-J | Peer-reviewed paper | CLM-062 | "Dunbar's number" is an upper-bound estimate; group function varies with context. |
| SRC-035 | Bowlby, J. (1969-1980). *Attachment and Loss* (Vols. 1-3). Basic Books. | various ISBNs | Book / developmental psychology | CLM-063 | Foundational; specific claims updated by later attachment research. |
| SRC-036 | Rockström, J., et al. (2009). "A safe operating space for humanity." *Nature*, 461. | doi.org/10.1038/461472a | Peer-reviewed paper | CLM-070, CLM-170 | Boundaries updated repeatedly; check most recent revision (SRC-037). |
| SRC-037 | Richardson, K., et al. (2023). "Earth beyond six of nine planetary boundaries." *Science Advances*, 9(37). | doi.org/10.1126/sciadv.adh2458 | Peer-reviewed paper | CLM-071 | Snapshot estimate; methodology continues to evolve. |
| SRC-038 | IPCC. (2023). *AR6 Synthesis Report*. | ipcc.ch/report/ar6/syr | Intergovernmental report | CLM-072, CLM-171 | Consensus document; conservative on tail risks. |
| SRC-039 | IPBES. (2019). *Global Assessment Report on Biodiversity and Ecosystem Services*. | doi.org/10.5281/zenodo.6417333 | Intergovernmental report | CLM-073 | Methodological caveats documented in the report. |
| SRC-040 | FAO. *The State of Food and Agriculture* (annual). | fao.org/publications/sofa | Intergovernmental report series | CLM-074 | Country-level data quality varies. |
| SRC-041 | IEA. *World Energy Outlook* (annual). | iea.org/reports/world-energy-outlook | Intergovernmental report series | CLM-075 | Scenario-based; assumptions disclosed. |
| SRC-042 | Zuboff, S. (2019). *The Age of Surveillance Capitalism*. PublicAffairs. | ISBN 978-1610395694 | Book / critical theory | CLM-080 | Critical lens; specific causal claims contested. |
| SRC-043 | O'Neil, C. (2016). *Weapons of Math Destruction*. Crown. | ISBN 978-0553418811 | Book / algorithmic harm | CLM-081 | Case studies; quantitative meta-evidence still developing. |
| SRC-044 | Eubanks, V. (2018). *Automating Inequality*. St. Martin's Press. | ISBN 978-1250074317 | Book / public-sector algorithms | CLM-082 | Ethnographic; not statistically generalizable but mechanism-rich. |
| SRC-045 | NIST. *AI Risk Management Framework* (NIST AI 100-1, 2023). | doi.org/10.6028/NIST.AI.100-1 | Government framework | CLM-083 | Voluntary; treat as starting point, not enforcement standard. |
| SRC-046 | Russell, S. (2019). *Human Compatible*. Viking. | ISBN 978-0525558613 | Book / AI safety | CLM-084 | Conceptual; empirical AI-risk benchmarks evolving fast. |
| SRC-047 | Tyler, T. R. (2006). *Why People Obey the Law*. Princeton University Press. | ISBN 978-0691126739 | Book / legal psychology | CLM-090, CLM-190 | Procedural-justice findings robustly replicated. |
| SRC-048 | Braithwaite, J. (2002). *Restorative Justice and Responsive Regulation*. Oxford University Press. | ISBN 978-0195136395 | Book / criminology | CLM-091 | Mixed empirical record by program design. |
| SRC-049 | Sherman, L. W., & Strang, H. (2007). *Restorative Justice: The Evidence*. Smith Institute. | smith-institute.org.uk | Meta-review | CLM-091 | Evidence quality varies by jurisdiction and offence type. |
| SRC-050 | World Bank. World Development Indicators. | databank.worldbank.org/source/world-development-indicators | Dataset | CLM-100, CLM-200 | Standard reference; country-level data quality varies. |
| SRC-051 | V-Dem Institute. Varieties of Democracy Dataset, most recent release. | v-dem.net | Dataset | CLM-101, CLM-201 | Expert-coded; coder-bias controls documented. |
| SRC-052 | Freedom House. *Freedom in the World*, most recent annual report. | freedomhouse.org | Index | CLM-102 | Methodology critiqued for Western framing; useful directional indicator. |
| SRC-053 | Our World in Data. | ourworldindata.org | Aggregator / dataset | many CLM-* | Curates other sources; check primary source for any specific claim. |
| SRC-054 | World Happiness Report (annual, Sustainable Development Solutions Network). | worldhappiness.report | Index / report | CLM-130 | Subjective wellbeing methodology limits cross-cultural comparison. |
| SRC-055 | Institute for Health Metrics and Evaluation. Global Burden of Disease Study. | healthdata.org/gbd | Dataset | CLM-131 | Comprehensive; estimation uncertainty disclosed. |
| SRC-056 | Schelling, T. C. (1978). *Micromotives and Macrobehavior*. W. W. Norton. | ISBN 978-0393090093 | Book / behavioral economics | CLM-150 | Foundational illustrations of emergent phenomena. |
| SRC-057 | Axelrod, R. (1984). *The Evolution of Cooperation*. Basic Books. | ISBN 978-0465021215 | Book / game theory | CLM-151 | Tit-for-tat result is robust; depends on stable interaction structure. |
| SRC-058 | Epstein, J. M., & Axtell, R. (1996). *Growing Artificial Societies*. Brookings / MIT. | ISBN 978-0262550253 | Book / agent-based modeling | CLM-152 | Demonstrative models, not predictive. |
| SRC-059 | Bonabeau, E. (2002). "Agent-based modeling: methods and techniques." *PNAS*, 99(suppl 3). | doi.org/10.1073/pnas.082080899 | Peer-reviewed paper | CLM-153 | Method overview; cited for ABM technique guidance. |
| SRC-060 | Snyder, T. (2017). *On Tyranny*. Tim Duggan Books. | ISBN 978-0804190114 | Pamphlet / political history | CLM-160 | Polemic; treat as illustrative, not statistically grounded. |
| SRC-061 | Mearsheimer, J. J. (2014). *The Tragedy of Great Power Politics* (updated ed.). W. W. Norton. | ISBN 978-0393349276 | Book / IR theory | CLM-200 | Realist lens; explicitly normative-theoretical. |
| SRC-062 | Walt, S. M. (1987). *The Origins of Alliances*. Cornell University Press. | ISBN 978-0801494185 | Book / IR theory | CLM-201 | Threat-balancing framework; case-study validation. |
| SRC-063 | Goldstone, J. A. (1991). *Revolution and Rebellion in the Early Modern World*. University of California Press. | ISBN 978-0520082670 | Book / historical sociology | CLM-031 | Pre-modern focus; later updates published. |
| SRC-064 | McNeill, J. R. (2000). *Something New Under the Sun*. W. W. Norton. | ISBN 978-0393321838 | Book / environmental history | CLM-170 | Twentieth-century focus; useful for ecological transition framing. |
| SRC-065 | Whitehouse, H., et al. (2019). "Complex societies precede moralizing gods throughout world history." *Nature*, 568. | doi.org/10.1038/s41586-019-1043-4 | Peer-reviewed paper | CLM-160 | Subject to subsequent re-analysis disputes; cite as contested. |
| SRC-066 | Henrich, J., et al. (2010). "The Weirdest People in the World?" *Behavioral and Brain Sciences*, 33(2-3). | doi.org/10.1017/S0140525X0999152X | Peer-reviewed paper + commentary | CLM-160 | Foundation for WEIRD literature. |
| SRC-067 | Lancet Commission on Global Mental Health and Sustainable Development. (2018). *The Lancet*, 392(10157). | doi.org/10.1016/S0140-6736(18)31612-X | Commission report | CLM-131, CLM-132 | Global synthesis; recommendations are normative. |
| SRC-068 | WHO. *World Mental Health Report* (2022). | who.int/publications/i/item/9789240049338 | Intergovernmental report | CLM-132 | Service-coverage data uneven by country. |
| SRC-069 | Bertrand, M., & Mullainathan, S. (2004). "Are Emily and Greg More Employable Than Lakisha and Jamal?" *AER*, 94(4). | doi.org/10.1257/0002828042002561 | Field experiment | CLM-191 | Replicated across jurisdictions and decades. |
| SRC-070 | Chetty, R., et al. Opportunity Insights (various papers). | opportunityinsights.org | Research program / datasets | CLM-110, CLM-111 | US-centric; methodology is open and well-documented. |
| SRC-071 | Goodhart, D. C. (1984). "Problems of monetary management: the UK experience." (Goodhart's law context). In *Monetary Theory and Practice*. | various | Book chapter | CLM-189 | Use the framing, not the specific monetary case. |
| SRC-072 | Campbell, D. T. (1979). "Assessing the impact of planned social change." *Evaluation and Program Planning*, 2(1). (Campbell's law). | doi.org/10.1016/0149-7189(79)90048-X | Peer-reviewed paper | CLM-189 | Pair with SRC-071 for measurement-distortion warnings. |
| SRC-073 | Diamond, J. (2005). *Collapse: How Societies Choose to Fail or Succeed*. Viking. | ISBN 978-0143036555 | Book / popular history | CLM-002 | Case selection criticized (Easter Island in particular); cite with caveats. |
| SRC-074 | Whyte, K. P. (2017). "Indigenous Climate Change Studies." *English Language Notes*, 55(1-2). | doi.org/10.1215/00138282-55.1-2.153 | Peer-reviewed paper | CLM-073, CLM-170 | Indigenous-led perspectives on environmental governance. |
| SRC-075 | Berkes, F. (2017). *Sacred Ecology* (4th ed.). Routledge. | ISBN 978-1138071490 | Book / commons / indigenous knowledge | CLM-011, CLM-074 | Strong on long-horizon commons cases. |
| SRC-076 | Beauchamp, T. L., & Childress, J. F. (2019). *Principles of Biomedical Ethics* (8th ed.). Oxford University Press. | ISBN 978-0190640873 | Textbook / ethics | CLM-130 | Standard reference for clinical-ethics principles. |
| SRC-077 | NIST. *Cybersecurity Framework* (CSF 2.0, 2024). | doi.org/10.6028/NIST.CSWP.29 | Government framework | CLM-085 | Voluntary; mapping required for any specific deployment. |
| SRC-078 | Cybersecurity & Infrastructure Security Agency (CISA). *Critical Infrastructure Sectors*. | cisa.gov/topics/critical-infrastructure-security-and-resilience | Government resource | CLM-085 | US-centric taxonomy; comparable lists exist for EU (NIS2) and others. |
| SRC-079 | EU. Regulation (EU) 2024/1689 ("AI Act"). | eur-lex.europa.eu | Regulation | CLM-083 | First comprehensive AI regulation; enforcement evolving. |
| SRC-080 | UN. Universal Declaration of Human Rights (1948); ICCPR (1966); ICESCR (1966). | un.org/en/about-us/universal-declaration-of-human-rights | Treaty / declaration | CLM-190 | Foundational rights instruments. |
| SRC-081 | International Idea. *Constitution-Building Database*. | constitutionnet.org | Database | CLM-101 | Comparative constitutional design reference. |
| SRC-082 | Tonry, M. (ed.). *Crime and Justice: A Review of Research* (annual series). University of Chicago Press. | journals.uchicago.edu/toc/cj | Edited review series | CLM-192 | High-quality synthesis; jurisdiction-specific. |
| SRC-083 | Sampson, R. J. (2012). *Great American City*. University of Chicago Press. | ISBN 978-0226734569 | Book / urban sociology | CLM-193 | Chicago-focused; mechanisms generalize, magnitudes do not. |
| SRC-084 | Holt-Lunstad, J., et al. (2010). "Social Relationships and Mortality Risk: A Meta-analytic Review." *PLOS Medicine*, 7(7). | doi.org/10.1371/journal.pmed.1000316 | Meta-analysis | CLM-042 | Earlier meta-analysis; companion to SRC-026. |
| SRC-085 | Cas Mudde. (2019). *The Far Right Today*. Polity. | ISBN 978-1509536856 | Book / political science | CLM-100 | Useful taxonomy; political stance disclosed by author. |
| SRC-086 | Boix, C. (2003). *Democracy and Redistribution*. Cambridge University Press. | ISBN 978-0521825605 | Book / political economy | CLM-110 | Formal model + cases; assumptions disclosed. |
| SRC-087 | Esping-Andersen, G. (1990). *The Three Worlds of Welfare Capitalism*. Princeton University Press. | ISBN 978-0691028576 | Book / comparative welfare | CLM-026, CLM-111 | Typology contested; data updated by later work. |
| SRC-088 | Heller, P., et al. (research program on participatory budgeting, Porto Alegre and beyond). Various papers. | unverified | Research program | CLM-018 | Replication mixed; durability depends on local conditions. |
| SRC-089 | Fishkin, J. S. (2018). *Democracy When the People Are Thinking*. Oxford University Press. | ISBN 978-0198820291 | Book / deliberative democracy | CLM-018, CLM-102 | Deliberative-poll evidence; selection effects flagged in the work. |
| SRC-090 | Yamagishi, T. (2011). *Trust: The Evolutionary Game of Mind and Society*. Springer. | ISBN 978-4431539353 | Book / social psychology | CLM-150 | Cross-cultural trust experiments; foundational. |
| SRC-091 | Brennan, J. (2016). *Against Democracy*. Princeton University Press. | ISBN 978-0691162607 | Book / political theory | CLM-018 | Cited as counterpoint (epistocracy critique); explicitly normative. |
| SRC-092 | World Values Survey. | worldvaluessurvey.org | Cross-country survey | CLM-150, CLM-160 | Wave-specific; useful for trend, not point estimates. |
| SRC-093 | Polity Project. *Polity 5 Dataset*. | systemicpeace.org/inscrdata.html | Dataset | CLM-101 | Aggregates regime characteristics; coder choices documented. |
| SRC-094 | Cingranelli, D., Richards, D., & Clay, K. C. *CIRIGHTS Dataset*. | cirights.com | Dataset | CLM-190 | Human-rights coding; coverage gaps documented. |
| SRC-095 | UNDP. *Human Development Report* (annual). | hdr.undp.org | Intergovernmental report | CLM-120 | HDI methodology disclosed; composite limits flagged. |
| SRC-096 | World Bank. *Worldwide Governance Indicators*. | govindicators.org | Index | CLM-100 | Aggregates expert perceptions; circularity caveats apply. |
| SRC-097 | Sen, A. (1999). *Development as Freedom*. Knopf. | ISBN 978-0385720274 | Book / capability approach | CLM-120 | Foundational for capability metrics. |
| SRC-098 | Nussbaum, M. (2011). *Creating Capabilities*. Belknap Press. | ISBN 978-0674050549 | Book / capability approach | CLM-120 | Specifies a list of central capabilities; the list itself is normative. |
| SRC-099 | Diener, E., et al. Subjective well-being research program (various). | unverified | Research program | CLM-130 | Caveats on measurement and cross-cultural comparability disclosed in primary papers. |
| SRC-100 | Stockholm International Peace Research Institute (SIPRI). *Yearbook* and military expenditure database. | sipri.org | Dataset / report | CLM-200, CLM-201 | Authoritative; some country reporting opaque. |
| SRC-101 | Sherman, L. W., et al. (2015). "Twelve experiments in restorative justice." *Journal of Experimental Criminology*, 11(4). | doi.org/10.1007/s11292-015-9247-6 | Meta-analysis | CLM-091, CLM-191 | Robust to within-experiment design. |
| SRC-102 | Goodin, R. E., et al. (2008). *Discretionary Time*. Cambridge University Press. | ISBN 978-0521709514 | Book / welfare regimes | CLM-026 | Time-as-resource framing; data limited to selected OECD countries. |

## Source Categories

- Historical and comparative civilization: SRC-001, SRC-002, SRC-003, SRC-004, SRC-005, SRC-009, SRC-010, SRC-063, SRC-064, SRC-073
- Governance and political theory: SRC-006, SRC-008, SRC-011, SRC-012, SRC-013, SRC-051, SRC-052, SRC-081, SRC-088, SRC-089, SRC-091, SRC-093, SRC-096
- Economics and inequality: SRC-014, SRC-015, SRC-016, SRC-017, SRC-018, SRC-019, SRC-020, SRC-021, SRC-022, SRC-070, SRC-086, SRC-087, SRC-095, SRC-097, SRC-098, SRC-102
- Public and mental health: SRC-023, SRC-024, SRC-025, SRC-026, SRC-027, SRC-055, SRC-067, SRC-068, SRC-076, SRC-084
- Education and learning: SRC-028, SRC-029, SRC-030, SRC-031
- Behavioral and social science: SRC-007, SRC-032, SRC-033, SRC-034, SRC-035, SRC-056, SRC-057, SRC-066, SRC-090, SRC-092
- Ecology and infrastructure: SRC-036, SRC-037, SRC-038, SRC-039, SRC-040, SRC-041, SRC-064, SRC-074, SRC-075
- Technology and AI governance: SRC-042, SRC-043, SRC-044, SRC-045, SRC-046, SRC-077, SRC-078, SRC-079
- Law, justice, and rights: SRC-047, SRC-048, SRC-049, SRC-080, SRC-082, SRC-083, SRC-094, SRC-101
- Defense and external relations: SRC-060, SRC-061, SRC-062, SRC-100
- Simulation and modeling: SRC-056, SRC-057, SRC-058, SRC-059
- Cross-country indicators: SRC-050, SRC-051, SRC-052, SRC-053, SRC-054

## Maintenance Notes

- New citations added by later iterations should continue the SRC-NNN sequence, never overwrite an existing ID.
- When a contested source is used as primary evidence, the corresponding claim must carry a `[CONTESTED]` tag in `evidence-matrix.md`.
- Sources marked `unverified` in URL/DOI must be resolved or replaced before this artifact moves to `reviewed`.
