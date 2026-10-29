# Expanded Qinming/Lepu UDI model coverage

## Scope and result

Expanded the original five-model identity resolution to **all 48 unique UDI-DI/model records returned for 乐普医学电子仪器股份有限公司**, unified social credit code **916100007197599584**, in the retrieved NMPA UDI company-search snapshot. This adds **43 model records**. All four result pages were retrieved (15/15/15/3), and every record has an official JSON export and matching HTML detail.

This is complete for that returned single-registrant result set, not a census of all Qinming aliases, predecessor registrations, manufacturers, historical versions or Chinese implantable devices. Original five-model and US-device files are preserved separately.

## Coverage

| Product group | UDI model records | Included models/families |
|---|---:|---|
| Cardiac pulse generators | 11 | Qinming2312M; Qinming8631D/DR; eight Qinming 8632 variants |
| Cardiac electrode leads | 15 | QM0228, QM0229, QM7211, QM7222 and QM7231, each with -45/-53/-60 entries |
| DBS pulse generator | 1 | LPB103 |
| DBS electrode assemblies | 3 | LPL201, LPL202, LPL203 |
| DBS extension-lead kit | 1 | LPE301 |
| External equipment | 6 | CK100P, CS800, HC600F, QM2353, FX300, QM8631 |
| Surgical tools and accessories | 11 | LPT401; QLP-7 through QLP-12; QLA-7/-8; YCX-1; QDLX-1 |
| **Total** | **48** | **12 active implanted devices; 19 implanted lead/component records; 17 external/procedural records** |

The eight 8632 model strings are preserved exactly: `Qinming 8632D`, `Qinming 8632Si`, `Qinming 8632SRi`, `Qinming 8632Di`, `Qinming 8632DRi`, `Qinming 8632SR`, `Qinming 8632S`, and `Qinming 8632DR`. Spacing, suffixes and raw Chinese spellings are not silently standardized. Family labels and English translations are curator annotations; the suffixes are not interpreted as verified pacing modes, MRI capabilities or physical dimensions.

The DBS descriptions cover a rechargeable stimulator and associated implanted electrodes/extension lead for STN stimulation in the stated Parkinson's-disease indication. Programmers, chargers, analyzers, surgical tools and introducer sheaths are not counted as implanted pulse generators. `YCX-1` is an external pacing-analyzer accessory, distinct from implanted DBS extension `LPE301`.

## Historical scope

**Twenty-three records were first published in June 2026**: eight 8632 generators, six QM0228/QM0229 leads, five implanted DBS records, and four external/procedural products (CK100P, CS800, HC600F, LPT401). They are explicitly flagged as outside the February 2024 review snapshot and highlighted in pale yellow in the workbook.

The remaining 25 have earlier UDI first-publication dates; that alone does not establish that their currently displayed fields were identical in February 2024. Neither first UDI publication nor version publication is treated as an original approval date or a certificate-renewal date. Embedded years in registration numbers are preserved as identifiers, not converted to approval dates.

## Provenance and checks

- **Exact matching:** all 48 search-result model/DI pairs match their official exports. Fourteen core fields per record also match the row-aligned public HTML detail, including model, product name, description, company identity, certificate strings and UDI dates.
- **Field provenance:** 22 copied source fields per model yield **1,056 provenance entries**, with JSON keys, detail links, export parameters and retrieval timestamps. These entries document copied fields; translated categories, family labels and uncertainty flags are separately identified annotations.
- **Raw evidence:** the ZIP retains 48 original JSON responses, 48 HTML detail responses, all four search-page responses, retrieval status, list rows, and a SHA-256 manifest. The packaged JSON also contains all official records, search logs and validation outcomes.
- **AI screen:** product descriptions were reviewed and screened for explicit Chinese/English AI/ML terminology. No explicit AI/ML mechanism was established. Software, programming functions and stimulation do not themselves establish AI; no firmware or detailed IFU audit was performed.

## Limits retained

**Nine records contain multiple certificate-number forms.** All are preserved verbatim; no historical equivalence or correction is inferred. Current registration validity, renewal history and commercial availability remain unverified. The prior provincial cross-check applies only to its documented product/registration-number pairs and is not extrapolated to all 48 records.

All 48 records state that instructions/labels contain no MR safety information; this is not an MR Unsafe determination. Blank retirement dates do not establish active marketing status. Company role remains registrant/filer rather than an inferred manufacturing-site role. No device values were imported from papers or secondary catalogs.

## Deliverables

The existing workbook now has **18 sheets**. Four expansion sheets open first: `Expanded UDI models`, `Expanded UDI provenance`, `Expanded UDI methods`, and `Expanded UDI searches`; all 14 earlier sheets remain intact.

- `qinming_expanded_udi_models.csv`: one row per unique UDI-DI/model, raw registry fields, translated category, component role, family annotation, prior-seed indicator, temporal scope, uncertainty flags and source links.
- `qinming_expanded_udi_provenance.csv`: 1,056 copied-field provenance rows.
- `qinming_expanded_official_exports.json`: all 48 official exports, retrieval parameters, source checksums and validation outcomes.
- `qinming_expanded_source_snapshots.zip`: original response bytes and checksum manifest.
