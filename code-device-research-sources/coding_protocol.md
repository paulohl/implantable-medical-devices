# Coding protocol and source register

## Scope and unit
A purposive pilot tied to the five cardiac-device cases in Leocadio (2024), DOI 10.5121/ijcsit.2024.02101. Read all 18 pages before selection. The paper is a narrative comparative analysis, not an original empirical dataset: p. 15 states, “No data were used in writing this paper, other than publicly available citations.” We therefore built a new claim-evidence corpus, not a reconstruction of participant data.

One row is one contiguous source excerpt. Quotes preserve words and punctuation; HTML entities are decoded and whitespace normalized. Superscript reference numbers are not included when outside the selected excerpt. Each row links to a source, textual locator and manuscript claim. Interpretation and codes are analyst judgments, not quotations. Source dates are distinct from retrieval date (28 October 2026). The corpus uses sources dated 2016–2023, rather than later evidence, to examine the paper on its own historical footing. Current web copies are not archived 2024 snapshots.

## Selection and access
Searches targeted the manuscript’s named devices and original manufacturer releases; the original Qinming clinical trial and a primary statute supply contrasting evidence types. Six documents were read as live full text. Four manufacturer releases are primary evidence of company claims and trial announcements, not independent confirmation. No historic archive sweep, systematic search, exhaustive screening or saturation claim was attempted. Wikisource and general historical archives do not fit this contemporary device question. No synthetic data or simulated quotes were used.

Publicly readable is NOT equivalent to openly licensed. S01, S02, S04 and S05 are free-to-read copyrighted releases; only short attributed excerpts are supplied. S03 is marked Open by the publisher, but its exact reuse licence was not verified. S06 contains public-domain US statutory text. A strictly open-licensed-only reuse corpus would need to exclude or replace the four corporate releases and resolve S03 licensing. Do not assume the whole dataset’s source text can be relicensed.

## Coding rules
Codes are nonexclusive. Apply only where the excerpt and its immediate source context justify them. Distinguish source assertion from trial observation, a projection from observed longevity, and regulatory status from actual adoption. No mention of AI means “not established in this source,” not “device has no AI.” Mechanism claims require a documented AI/ML function, ideally training/validation and computation location; an automated pacing algorithm or implant-to-implant communication alone is insufficient.

Relations: **supports_noncausal** = supports the narrower device claim but not a causal AI benefit; **qualifies** = narrows its scope, design or interpretation; **contradicts** = directly conflicts with a factual identifier; **supports_context** = primary contextual legal evidence, not device-specific validation.

| Code | Operational definition | Derived from paper |
|---|---|---|
| AI_EXPLICIT | Source expressly calls a function AI or ML; do not infer from automatic or adaptive. | §3.2; §8.2 |
| AUTOMATION | Automatic algorithmic behavior without established learned-model provenance. | §4.4; §5.1 |
| LOCUS | Where computation/filtering is described; unknown if not directly specified. | §3.1–3.2 |
| DIAGNOSTIC | Arrhythmia detection/filtering, not therapy or patient outcome. | §3.2; §8.1 |
| THERAPY | Direct pacing or treatment coordination. | §4.4–4.7 |
| LONGEVITY | Battery/service life or need for long-term follow-up. | §4.4; §7.1 |
| PROJECTION | Modeled/expected future outcome, not observed follow-up. | §4.4; §5.3 |
| TRIAL_DESIGN | Design, comparator, enrollment or follow-up supporting inference limits. | §4.5; §4.7 |
| CLINICAL_ENDPOINT | Reported clinical/device endpoint or prespecified endpoint, not AI attribution. | §4; §5 |
| QUANT_CLAIM | Numerical performance assertion; retain denominator and evidence type. | §4; §5 |
| IDENTITY | Correct device/model/component attribution. | §4.5–4.6; §5 |
| INTEROPERABILITY | Device communication; not by itself EHR interoperability or AI. | §4.6; §6.1 |
| ADOPTION_STAGE | Investigational, planned enrollment, or availability at source date. | §4; §6 |
| REGULATORY | Approval report, investigational constraint or legal requirement. | §4; §6.1 |
| CYBERSECURITY | Security obligations or scope of qualifying devices. | §6.1 |
| SCOPE_LIMIT | Footnote, limitation, comparator or boundary narrowing an inference. | §5–7 |

## Source register

### S01 — BIOMONITOR IV
- Creator: BIOTRONIK. Date: 2023-06-12.
- Title: BIOTRONIK announced first implant of new implantable cardiac monitor with artificial intelligence, targeting efficiency in monitoring for cardiac arrhythmias.
- URL: https://www.prnewswire.com/news-releases/biotronik-announced-first-implant-of-new-implantable-cardiac-monitor-with-artificial-intelligence-targeting-efficiency-in-monitoring-for-cardiac-arrhythmias-301848638.html
- Relation to paper: Cited in manuscript pp. 15–16.
- Type and limitations: Manufacturer press release; Manufacturer; performance based on data on file.
- Rights: Publicly readable; copyrighted; no open reuse licence verified.
- Access: Full text read with web_fetch; automated re-fetch succeeded. Retrieved 2026-10-28.

### S02 — Micra AV2 / Micra VR2
- Creator: Medtronic plc. Date: 2023-05-01.
- Title: Medtronic receives FDA approval for its next generation Micra leadless pacing systems.
- URL: https://news.medtronic.com/2023-05-01-Medtronic-receives-FDA-approval-for-its-next-generation-Micra-leadless-pacing-systems
- Relation to paper: Original manufacturer release behind manuscript’s Wainscot Media citation.
- Type and limitations: Manufacturer press release; Manufacturer; longevity projection references internal modeling.
- Rights: Publicly readable; copyrighted; no open reuse licence verified.
- Access: Full text read with web_fetch; automated re-fetch succeeded. Retrieved 2026-10-28.

### S03 — Qinming8631 DR (QM7211 is ventricular lead)
- Creator: Xiang, Mei-Xiang; Wang, Dong-Qi; Xu, Jing; et al.. Date: 2016-11-20.
- Title: Evaluation of Safety and Efficacy of Qinming8631 DR Implantable Cardiac Pacemaker in Chinese Patients: A Prospective, Multicenter, Randomized Controlled Trial of the First Domestically Developed Pacemaker of China.
- URL: https://journals.lww.com/cmj/fulltext/2016/11200/evaluation_of_safety_and_efficacy_of_qinming8631.3.aspx
- Relation to paper: Xiang et al. cited in manuscript p. 18; corrected DOI 10.4103/0366-6999.193443; PMCID PMC5126155.
- Type and limitations: Original randomized clinical trial; Authors report no sponsorship and no conflicts; short follow-up.
- Rights: Publisher marks article Open; copyright Chinese Medical Association; exact reuse licence not verified.
- Access: Full text read with web_fetch; automated re-fetch unavailable. Retrieved 2026-10-28.

### S04 — EMBLEM MRI S-ICD + EMPOWER MPS
- Creator: Boston Scientific Corporation. Date: 2021-12-02.
- Title: Boston Scientific Initiates Trial to Evaluate Industry's First Modular CRM System.
- URL: https://news.bostonscientific.com/2021-12-02-Boston-Scientific-Initiates-Trial-to-Evaluate-Industrys-First-Modular-CRM-System
- Relation to paper: Primary sponsor source replacing manuscript’s Prutchi blog report.
- Type and limitations: Manufacturer trial-initiation announcement; Sponsor; prospective plans, not completed clinical results.
- Rights: Publicly readable; copyrighted; no open reuse licence verified.
- Access: Full text read with web_fetch; automated re-fetch succeeded. Retrieved 2026-10-28.

### S05 — AVEIR DR i2i
- Creator: Abbott. Date: 2023-05-20.
- Title: Abbott Unveils Late-Breaking Data Showing the World's First Dual-Chamber Leadless Pacemaker Study Met All Three Primary Endpoints.
- URL: https://abbott.mediaroom.com/2023-05-20-Abbott-Unveils-Late-Breaking-Data-Showing-the-Worlds-First-Dual-Chamber-Leadless-Pacemaker-Study-Met-All-Three-Primary-Endpoints
- Relation to paper: Directly cited in manuscript p. 15; figures reproduced pp. 8–9.
- Type and limitations: Sponsor report of clinical trial results; Sponsor summary, not independently reanalyzed patient data.
- Rights: Publicly readable; copyrighted; no open reuse licence verified.
- Access: Full text read with web_fetch; automated re-fetch succeeded. Retrieved 2026-10-28.

### S06 — Qualifying cyber devices (cross-cutting)
- Creator: United States Congress. Date: 2022-12-29.
- Title: 21 U.S.C. § 360n–2: Ensuring cybersecurity of devices (FD&C Act § 524B).
- URL: https://www.law.cornell.edu/uscode/text/21/360n-2
- Relation to paper: Added primary legal evidence for manuscript §6.1.
- Type and limitations: Primary statute, reproduced by Cornell LII; Legal obligation, not evidence of clinical effectiveness.
- Rights: Underlying US statutory text public domain; LII editorial material not reproduced.
- Access: Full text read with web_fetch; automated re-fetch succeeded. Retrieved 2026-10-28.

## Data dictionary and quality checks
**Passages / CSV:** passage and source IDs; device; paper anchor; quote locator; verbatim quote; semicolon-delimited codes; claim relation; interpretation; metric; sample size; follow-up; source bibliographic metadata; rights; AI status; processing locus; bias; verification method; automated check. Blank metric/sample/follow-up means not applicable or not stated for the excerpt, never zero. Sample/follow-up fields may carry context from elsewhere in the same source; they are not additional verbatim text.

**Sources:** six records with creator, date, title, URL, type, rights, relation to the paper, AI status, processing locus and bias. Retrieval hashes identify the HTML obtained for the automated audit, not immutable historical document versions.

**Codebook:** 16 operational codes. This is a single-pass, single-coder pilot; no independent second coder or inter-rater reliability estimate. Passages are nested within documents; passage counts are not independent study counts or prevalence estimates. No pooled effect or device ranking is valid across these different endpoints. Equity, consent, EHR integration and measured AI adoption remain evidence gaps, not negative findings.

**Access limitations:** PMC and PubMed returned browser-check pages; the Qinming trial was read in full from its open publisher copy (LWW redirects to Ovid). No numerical table cells were extracted; quantitative excerpts come from source prose.

**Automated checks:** 18/22 excerpts matched a second direct HTML retrieval after entity/whitespace normalization. Remaining excerpts were checked against the full text returned by web_fetch. Unique IDs, source links, code membership and XLSX row count validated; workbook contains no formulas.
