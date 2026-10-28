# Implantable AI devices: official-record map

**Scope:** A bounded, paper-seeded map of implantable cardiac devices and their public regulatory, UDI and clinical-trial records. Retrieved 28 October 2026. No simulated data or device values copied from papers.

## What this map establishes

- **Six verified device/system entries**, linked to **eight exact-identity official records** and one separately marked, family-level contextual trial record. These are not six independent approvals: Micra AV2 and VR2 share a supplement.
- **AI integration is not established by the reviewed official record content.** All six entries are flagged accordingly. This is a limitation of the evidence reviewed, not proof that a device does not use AI. Automatic arrhythmia detection, AV synchrony, rate responsiveness and implant-to-implant communication were not relabeled as AI.
- **Manufacturer identity is not assumed from sponsorship or an application.** BIOMONITOR IV has an explicit manufacturer in its FDA summary. Other company fields preserve their verified role as applicant or trial sponsor.
- **Two unresolved Qinming search seeds** remain outside the verified device table. The paper alternates between 8631 variants in section 4.5 and QM7211 in section 5; these names were not merged.

## Adaptation to your paper

Leocadio, *Advancements in Implantable Medical Devices…* (2024), DOI [10.5121/ijcsit.2024.02101](https://doi.org/10.5121/ijcsit.2024.02101), is a narrative review. Its data-availability statement explicitly says no data were used other than publicly available citations (p15). Consequently, this is an independently assembled record map—not a reconstruction of an underlying cohort or a meta-analysis.

The search seeds came from BIOTRONIK/BIOMONITOR IV (section 3.2 and references), Micra AV2/VR2 (section 4.4), Qinming 8631/QM7211 (sections 4.5 and 5), EMBLEM/EMPOWER (section 4.6), and AVEIR DR i2i (section 4.7). Neural implants and other broad background references were not expanded into a global device inventory. The original paper supplies scope only, not the values in the dataset.

## Sources and inclusion rules

| Repository | Record type | Why it belongs |
|---|---|---|
| FDA openFDA 510(k) | Clearance decision | Regulatory identity, applicant and decision date |
| FDA openFDA PMA | Approval supplement or manufacturing notice | Specific model/system decision scope; supplement IDs retained |
| FDA-hosted K230375 summary | Regulatory submission document | Explicit BIOMONITOR manufacturer and intended function |
| NLM AccessGUDID | UDI device listing | Exact BIOMONITOR IV model, company and clearance linkage |
| ClinicalTrials.gov API v2 | Trial registration | Named system, sponsor, study status and enrollment with actual/estimated distinction |

**Tier A (core):** a stable official identifier and explicit named-device match. **Tier B (context only):** NCT04075084 describes BIOMONITOR III and possible successors; it is not treated as IV-specific evidence. Excluded: unrelated Qinming/acupuncture results, empty searches, unsupported manufacturer/model guesses, press-release values and paper-reported clinical outcomes. Quality tiers concern identity/provenance, not trial risk of bias or device safety.

Seven ClinicalTrials.gov name searches and four bounded FDA name searches are logged, with their saved responses. Direct official-ID retrievals are separately recorded by URL in the record table and archive. Search pages were capped at 10 trial or 3 FDA hits; returned counts are not exhaustive totals. No paid or authenticated sources were used.

## Important distinctions

1. **Clearance versus approval:** BIOMONITOR IV K230375 is a 510(k) clearance dated 2023-05-19. Micra P150033S161 is an approval supplement dated 2023-04-20, shared by AV2/VR2. AVEIR DR P150035S003 is dated 2023-06-29. EMBLEM P110042S043 is dated 2015-03-13. These dates are decision dates, not launch dates.
2. **Supplement scope:** Micra P150033S209 is a 2025 manufacturing notice used only to verify model mappings MC2AVR1/MC2VR01. It is not their initial approval and postdates the paper. EMBLEM approval is not evidence of approval for the combined EMPOWER/EMBLEM configuration.
3. **EMPOWER evidence:** NCT04798768 directly names both components and describes an EMBLEM S-ICD upgraded with investigational firmware. No matching EMPOWER marketing decision was established by the limited FDA name search. This does not establish current approval status in every jurisdiction.
4. **Trial enrollment is not an outcome:** AVEIR DR i2i NCT05252702 currently records 464 actual participants; MODULAR ATP NCT04798768 records 297 actual participants. These are registry-wide counts, not efficacy denominators and not substitutes for the paper's early AVEIR analysis of 300 people. NCT04075084 lists 1,400 estimated participants and is family context only.
5. **Current snapshot, not historical reconstruction:** registry statuses and listing versions can postdate February 2024. Decision dates are historical events; company names and trial status are from current retrieved records. No historical registry-version audit was performed.
6. **AI evidence remains unresolved:** no technical inference was made about model architecture, training, adaptation, or where computation occurs (implant versus external system/cloud). The reviewed K230375 summary describes arrhythmia recording and remote monitoring but does not explicitly identify AI/ML. Broader labeling and software documentation may resolve this.

## Deliverables and row units

- `implantable_ai_map.xlsx` — six filterable sheets: Devices (6 rows), Repository records (9), Field provenance (70), Unresolved seeds (2), Search log (11), and Data dictionary (15 fields).
- `implantable_devices.csv` — one row per verified named device/system; local D01–D06 keys are not official IDs. This is the harmonized research index.
- `repository_records.csv` — one row per distinct official record. Use this table, not device rows, to count unique regulatory records. Shared links use semicolons.
- `field_provenance.csv` — field-level source values with source-record ID, JSON path or PDF page, and repository/context classification. Curator interpretations are identified in the data dictionary rather than presented as source assertions.
- `official_source_snapshots.zip` — raw JSON responses, FDA summary PDF, source URLs, search log and SHA-256 manifest. These preserve what was retrieved if live records change.

**Missingness:** blank fields mean not established in this bounded review, never zero or not applicable. IDs are text; dates use ISO format. The workbook uses no formulas. Source URLs are clickable. AI flags, device classes and interpretations are curator annotations; official company names, IDs, dates, models and counts retain repository provenance.

**Checks completed:** unique official record IDs; valid device/record links; provenance IDs resolve to retained source files; model strings retained; six workbook sheets readable; no Excel error cells. No patient-level data are included. Official provenance does not independently validate sponsor submissions or FDA submission claims.

## Remaining gaps and the fastest extensions

- Resolve Qinming identities through China's NMPA and Chinese UDI records, including original-language legal names; US no-match searches cannot resolve Chinese registration.
- Inspect device labeling, software descriptions and regulatory AI listings to determine whether AI is confirmed and whether it executes in the implant, programmer, or cloud.
- Expand exact UDI model coverage for the other systems and build a historical February 2024 snapshot separately from current records.

## Reuse

This dataset points to public US federal repositories and preserves their records for audit. No blanket license is asserted over manufacturer-authored submission material. Check source-specific terms before redistributing document content; the archive retains source attribution and retrieval timestamps.
