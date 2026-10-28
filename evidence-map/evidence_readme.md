# Implantable-device evidence map

**Bottom line:** the paper supports a function-stratified evidence map, not a ranking of “best AI implants.” It is a narrative review with no original dataset (p.15). Six candidate systems/models across five manufacturers were extracted. No reviewed comparison isolates the clinical contribution of AI.

## What the comparison shows

| Candidate | Most useful extracted evidence | Certainty and boundary |
|---|---|---|
| BIOMONITOR IV | Cited manufacturer release: 86% fewer false-positive detections while preserving 98% of true episodes | Very low; data on file, AF filter “Very Specific”; AI applies only to AF. Comparator is without SmartECG, not an AI-only ablation. |
| Micra AV2 | Nearly 16-year median projected longevity; review also says 8–13 years | Very low for longevity claim; projection, not observed long-term follow-up. |
| Micra VR2 | Nearly 17-year median projected longevity; review also says 12 years | Very low for longevity claim; conflicting review specifications retained. |
| Qinming8631 DR | Cited randomized trial: effective pacing 81.4% versus 79.5% with Talos DR in full analysis set, six months | Low for this endpoint; missing assessments/attrition and reporting limitations. Noninferiority does not establish superiority or an AI benefit. |
| EMBLEM S-ICD + EMPOWER | Coordinated defibrillation and leadless pacing/ATP described | Very low; no numerical clinical performance result in review or checked trial-initiation report. |
| AVEIR DR | 98.3% implant success; >97% of patients with successful AV synchrony; mean synchrony >95% in each of seven activity conditions | Low for short-term descriptive performance; single arm, 300 initially enrolled, 55 centers, three months. These percentages measure different things. |

## Corrections that matter

- **Qinming identity:** QM7211 is the ventricular lead in the cited trial, not the dual-chamber pacemaker. The candidate is Qinming8631 DR.
- **Boston component boundaries:** the S-ICD is extrathoracic; the leadless pacemaker is intracardiac. “Cannot defibrillate” applies to the pacemaker component, not the combined system.
- **Longevity:** the Micra figures are projections. The review’s conflicting values remain visible rather than being averaged or silently replaced.
- **AI versus automation:** automatic synchrony, rate response and implant-to-implant communication do not by themselves establish a machine-learning implementation or its added clinical benefit.

## How to use the files

The Excel workbook has five filterable sheets: **Candidates**, **Evidence**, **Methods**, **Issues**, and **Sources**. Start with Candidates; use Evidence for atomic claims and exact source conditions. The CSV is the same long-form Evidence sheet for reuse. Source IDs and URLs distinguish claims printed in the supplied review from extra details recovered from its cited sources. Page references are printed PDF page numbers.

Percentages use a 0–100 numeric scale. Approximate values and inequalities retain their qualifiers. Units are years, months, g, beats/min, V and ms. No drugs or dose regimens are compared, so the recipe’s dose normalization was replaced with device-setting extraction. Missing settings are **NR**, not zero; protocol acceptance thresholds are not performance outcomes.

## GRADE-lite and limits

This is a pragmatic endpoint-level certainty assessment, not formal GRADE. Randomized evidence starts High, prospective single-arm evidence Low, and narrative/manufacturer/data-on-file claims Very low. Serious bias, inconsistency, indirectness, imprecision or selective reporting can lower certainty, with a Very low floor. Qinming’s six-month pacing endpoint is downgraded twice from High to Low; its trial does not test AI. AVEIR’s short-term single-arm performance remains Low, while its unquantified safety pass/fail claim is Very low. Protocol settings are Not applicable. “Not demonstrated” means AI validation was not established in the checked materials, not that the device has no AI.

No numeric overall score, cross-indication safety ranking, pooled effect estimate, or recommendation is justified. Five cited web sources were checked, including the Qinming full trial; this is not an exhaustive search or an audit of current regulatory status. The Qinming source itself contains inconsistencies in reported between-group differences and pulse-width descriptions; the workbook flags them and does not propagate questionable effect estimates. No synthetic patient data were used.

## Checked sources

- **P: Leocadio (2024), supplied review** — https://doi.org/10.5121/ijcsit.2024.02101
- **B: BIOTRONIK (2023-06-12), manufacturer release** — https://www.prnewswire.com/news-releases/biotronik-announced-first-implant-of-new-implantable-cardiac-monitor-with-artificial-intelligence-targeting-efficiency-in-monitoring-for-cardiac-arrhythmias-301848638.html
- **M: Wainscot Media (2023-05-01), manufacturer announcement coverage** — https://www.dicardiology.com/content/medtronic-receives-fda-approval-its-next-generation-micra-leadless-pacing-systems
- **Q: Xiang et al. (2016), randomized noninferiority trial** — https://pmc.ncbi.nlm.nih.gov/articles/PMC5126155/
- **A: Abbott (2023-05-20), manufacturer trial-results release** — https://abbott.mediaroom.com/2023-05-20-Abbott-Unveils-Late-Breaking-Data-Showing-the-Worlds-First-Dual-Chamber-Leadless-Pacemaker-Study-Met-All-Three-Primary-Endpoints
- **S: Prutchi (2021-12-13), trial-initiation report** — https://www.implantable-device.com/2021/12/13/boston-scientific-starts-trial-of-emblem-s-icd-with-empower-leadless-pacemaker/
