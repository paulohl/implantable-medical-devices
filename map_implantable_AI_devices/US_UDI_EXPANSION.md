# US UDI coverage expansion

Retrieved 29 October 2026 from AccessGUDID's public search and official v3 lookup endpoints. This extends the original map beyond the Chinese single-registrant expansion to the BIOMONITOR, Micra, AVEIR, EMBLEM and EMPOWER cardiac-device search families.

## Coverage

**44 accepted primary-DI records represent 36 exact labeler/model pairs.** These are two different counting units; repeated model strings across primary DIs are preserved rather than silently deduplicated.

| Family | Primary-DI records | Exact labeler/model pairs | Included scope |
|---|---:|---:|---|
| BIOMONITOR | 8 | 8 | Six implanted cardiac-monitor records; insertion kit and Remote Assistant |
| Micra | 6 | 5 | Five implanted pacemaker DI records covering four model labels; one introducer |
| AVEIR | 14 | 14 | Five implanted pacemaker models; nine delivery, retrieval, programming, transmission or software records |
| EMBLEM | 16 | 9 | Two ICD generators; three electrode DI records; eleven programmer, insertion, delivery, screening or data-card records |
| EMPOWER cardiac pacemaker | 0 verified | 0 verified | No qualifying match established by the documented narrowed searches |
| **Total accepted** | **44** | **36** | **18 active implanted DI records, three implanted electrode DI records, 23 nonimplanted records** |

Combined with the preserved 48-row Chinese expansion, the two expansion tables contain **92 primary-DI records**. BIOMONITOR IV's DI was already in the original US snapshot, so this extension contributes 43 other US primary DIs rather than 44 wholly new identities. It does not add 44 newly verified AI devices or establish 44 distinct approvals.

## Model details worth retaining

- **Micra:** `MC2AVR1` (AV2), `MC2VR01` (VR2), `MC1AVR1` (AV), and `MC1VR01US`; the last has two primary DIs with different source-reported distribution statuses. Introducer `MI2355A` is not a pacemaker.
- **AVEIR:** implanted models `LSP112V`, `LSP201A`, `LSP202V`, `LSP203A` and `LSP203V`. Source descriptions label the latter two “AR 2 Leadless Pacemaker” and “VR MINI Leadless Pacemaker.” These descriptions are not evidence of approval dates, AI, or retrospective membership in the original DR configuration.
- **EMBLEM:** generators `A209` and `A219`; electrode models `3401` and `3501`. Model `3200` appears under six primary DIs. Data card `3205` has brand `NA`, but its official description explicitly identifies the EMBLEM programmer, so it is retained as an accessory.
- **BIOMONITOR:** raw model strings include `471155` (IV), `450218` (IIIm), `436066` (III), `398493` (2-AF), `2-S`, and `394119`, plus the insertion kit and Remote Assistant. Raw version/model strings are not replaced by inferred commercial generations.

The workbook's `US UDI model index` groups exact labeler/model pairs and lists all retained primary DIs. It is an index, not a claim that those DIs are interchangeable.

## Search, inclusion and provenance

The single-term family searches returned 9 BIOMONITOR, 8 Micra, 14 AVEIR and 16 EMBLEM candidates. Queries used `page_size=100` to retrieve each entire small result set in one response; default 10-row pagination showed order variation and was not used to claim complete coverage.

For EMPOWER, three narrowed queries were exhausted: `EMPOWER AND "BOSTON SCIENTIFIC"` returned one unrelated LithoVue Empower record; `EMPOWER AND pacemaker` and `EMPOWER AND leadless` each returned zero. This is a bounded no-match result, not proof that no EMPOWER cardiac device has a UDI anywhere or a statement about its regulatory status.

All **48 distinct candidates** were downloaded from the official lookup endpoint, including rejected matches. Search model, labeler and public-record UUID were checked against the lookup response. **Four exclusions** are documented: an unrelated Noraxon BioMonitor sensor, two microbiological *P. micra* controls and the LithoVue device. No paper-derived product values were used.

The accepted records have **1,188 field-provenance entries**: 27 raw fields per record, with exact JSON paths and retrieval URLs/timestamps. Complete identifier arrays preserve package, previous and primary identifier roles; package IDs are not counted as separate model rows. Raw official responses and SHA-256 checksums are retained in the source archive.

## Important qualifications

**Historical dates:** five accepted AVEIR records were first published after February 2024: LSRM01, LSRMC01 and LSRM1000 in December 2024; LSP203A in August 2025; LSP203V in September 2026. These are flagged and highlighted in the workbook. GUDID publication, version and distribution-end dates are not clearance/approval dates; current fields on older records are not reconstructed February 2024 values.

**Company role:** `companyName` is retained as GUDID labeler. In particular, AVEIR records name **ST. JUDE MEDICAL, INC.**, not an automatically substituted parent-company name. Labeler, applicant, sponsor and manufacturing site remain distinct roles.

**Distribution status:** the registry reports 39 accepted records “In Commercial Distribution” and five “Not in Commercial Distribution.” These are source-reported statuses, not independent conclusions about current sales, approval validity, recall status or safety.

**Electrode terminology discrepancy:** three EMBLEM electrode records describe subcutaneous electrodes but carry the GMDN term “Endocardial defibrillation lead.” Both source fields are preserved and the discrepancy is flagged; no endocardial placement is inferred from that generic term.

**AI:** this is an identity/UDI expansion. It does not alter the earlier AI review. BIOMONITOR IV's confirmed external SmartECG AI is not generalized to other BIOMONITOR generations or to onboard processing. Other devices are not relabeled as AI solely because they have software or automatic functions.

## Files

The workbook now contains **24 sheets**, with six US UDI sheets first; all 18 prior sheets were value-checked as unchanged. The US tables remain separate from the Chinese registry tables so that source schemas, company roles and date semantics remain explicit.

- `us_expanded_udi_records.csv`: 44 accepted primary-DI records with raw registry fields, component annotations, temporal qualifications and source links.
- `us_expanded_udi_provenance.csv`: 1,188 raw-field provenance entries.
- `us_expanded_udi_exclusions.csv`: four rejected keyword matches and reasons.
- `us_expanded_official_exports.json`: all 48 candidate lookup responses, inclusion decisions, search logs and methods.
- `us_expanded_source_snapshots.zip`: original lookup and final search responses, retrieval logs, candidates and checksum manifest.
