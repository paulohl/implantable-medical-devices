# Qinming resolved through Chinese regulatory records

**Finding:** NMPA's Chinese UDI database identifies **two Qinming8631 pacemaker models and three QM7211 electrode-lead models**. QM7211 is not a competing pacemaker model. The paper's two search seeds therefore describe different components and must not be merged.

Retrieved 28 October 2026. Values below come from official registry exports, not papers, distributor catalogs or procurement search snippets.

## Exact model identities

| Official model | Product category, translated | Minimum-sales-unit UDI-DI | NMPA record |
|---|---|---|---|
| Qinming8631D | Implantable cardiac pacemaker | `06942807604057` | [Official record](https://udi.nmpa.gov.cn/showDetailCX.html?deviceRecordKey=6a4ad7d3-d238-4305-a796-aff92a2dfe5e) |
| Qinming8631DR | Implantable cardiac pacemaker | `06942807604040` | [Official record](https://udi.nmpa.gov.cn/showDetailCX.html?deviceRecordKey=43b5a3d8-98c4-4461-830b-f74572edaaec) |
| QM7211-45 | Implantable pacemaker electrode lead | `06942807605108` | [Official record](https://udi.nmpa.gov.cn/showDetailCX.html?deviceRecordKey=696504a7-e877-4485-b7cb-59f74eeddf78) |
| QM7211-53 | Implantable pacemaker electrode lead | `06942807605092` | [Official record](https://udi.nmpa.gov.cn/showDetailCX.html?deviceRecordKey=c343c793-e3a2-4a13-aeef-4bd24591f662) |
| QM7211-60 | Implantable pacemaker electrode lead | `06942807605030` | [Official record](https://udi.nmpa.gov.cn/showDetailCX.html?deviceRecordKey=64d7d4a7-4788-4662-a5bd-f237bbb5e7a4) |

The pacemaker's raw Chinese name is **植入式心脏起博器**, including the registry's spelling. The lead name is **植入式心脏起搏器电极导线**. Translations and categories are separate annotations; raw names are preserved.

## Legal company and product function

All five records name **乐普医学电子仪器股份有限公司** as the medical-device registrant/filer and give unified social credit code **916100007197599584**. The registered English-name field is blank, so no unofficial English translation is substituted as a verified legal name. “Qinming” is retained as model branding. Formal predecessor-name changes and parent-company ownership were not independently established from a corporate registry.

The generator descriptions list a battery, circuitry, housing, sealing plug and electrode connector, for treatment of bradyarrhythmia. The QM7211 descriptions specify a lead and accessories with connector, conductor body, suture sleeve, ring electrode, helical electrode tip and drug plug; the lead works with a compatible pacemaker to provide pacing and sensing in the right atrium or ventricle. These are distinct device types: registry classification codes **12-01-01** and **12-01-04**, respectively.

**AI status:** no explicit AI/ML mechanism is established in the retrieved descriptions. The identity correction does not verify AI integration. No trained-model, firmware or detailed IFU audit was performed.

## Registration numbers: preserve both forms

| Product family | Numbers listed together in UDI records | Independently corroborated by provincial regulator |
|---|---|---|
| Qinming8631D/DR | 国械注准20163121585 and 国械注准20163211585 | 国械注准20163121585 |
| QM7211 leads | 国械注准20163121583 and 国械注准20163211583 | 国械注准20163121583 |

The [Shaanxi Medical Products Administration's Q3 2025 export-sales certificate notice](https://mpa.shaanxi.gov.cn/sxsypjdglj/jgxx/rcjgxx/202511/t20251128_3589768.html), published 28 November 2025, independently links each corroborated registration number to the corresponding product category and the same Chinese company. The row-level cross-checks are retained in the workbook and JSON.

**Unresolved:** whether the additional `2016321…` forms are historical numbers, recoded numbers or data errors. Both are preserved verbatim; neither is silently corrected or declared equivalent. The NMPA registration-search portal returned HTTP 412, so current certificate validity and renewal history remain unverified.

## Dates and availability must not be conflated

- **2020-09-07:** UDI product-identifier publication date, not original approval date.
- **2022-04-19:** public UDI version date (version 3), not a renewal date.
- **2026-05-30** (pacemaker) and **2026-09-26** (lead): export-sales certificate expiry dates in the provincial notice, not verified device-registration expiry dates. Both dates precede retrieval; no later export certificate or renewal was established.
- **Blank retirement date / `--` listing status:** not proof of current commercial distribution, non-withdrawal or valid marketing authorization.
- **MR information:** the registry states that the instructions/label contain no MR safety information. This is not equivalent to an MR Unsafe determination.

## Search and quality checks

A basic UDI query for `8631` or `QM7211` returned zero rows, but the Chinese company-name search returned 48 records. All four pages were retrieved; exact model matches were then followed to their public detail records and official JSON downloads. This demonstrates why the initial zero-hit model searches cannot be interpreted as absence.

The underlying public form uses `POST /getDeviceList.html`. Official exports use `POST /toDown.html` with the exact `deviceRecordKey` and `type=2`. The site's JSON wrapper reports `success=false` even when valid rows are populated; inclusion used the actual matched rows and independently retrieved detail/export content, not that flag. No login or access-control bypass was used.

Only the five exact matches were retained. Unrelated company records, newer 8632 devices, secondary procurement snippets, search-only NMPA notices and unverified corporate histories were excluded from product-field evidence. The general NMPA search portal and an approval-document delivery notice returned HTTP 412; two procurement PDF hosts failed DNS resolution. Neither limitation prevents the five direct UDI matches, but certificate validity remains a separate gap.

## Files and integration

The workbook now opens on `Qinming registry`, with additional `Qinming provenance`, `Qinming cross-check`, `Qinming methods` and `Qinming searches` sheets. The original unresolved-seed rows now point to the resolution. Other original repository data and AI-verification results are retained.

- `qinming_registry_records.csv`: five exact UDI/model rows with raw Chinese fields, translated product categories, certificate-number qualifications and source links.
- `qinming_field_provenance.csv`: 70 field-level entries linked to original export keys and URLs.
- `qinming_official_exports.json`: five complete official JSON records, two provincial cross-check rows, search parameters and methods. Original-response SHA-256 digests are supplied for audit; the JSON object is packaged rather than a byte-identical concatenation of downloads.

**Counting rule:** these are five model records but only two pacemaker models; the other three are electrode leads. They are not five newly verified AI devices. Original six-device CSV files remain the initial snapshot; this is an explicitly separate Chinese-registry extension.
