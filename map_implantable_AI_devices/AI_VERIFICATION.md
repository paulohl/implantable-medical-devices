# Which mapped devices actually use AI?

Verified 28 October 2026. **One of the six entries has explicit evidence of AI in its associated monitoring system: BIOMONITOR IV with SmartECG. The described AI is external, not inside the implant.** AI use is not verified for the other five entries; that is not proof of absence.

## Device-by-device verdicts

| Device/system | Verdict | What the evidence actually supports |
|---|---|---|
| BIOMONITOR IV with SmartECG | **AI confirmed in external monitoring** | BIOTRONIK explicitly identifies AI for AF analysis. SmartECG executes in the Home Monitoring Service Center (HMSC), not the implant or interrogation programmer. |
| Micra AV2 | **AI not verified; conflicting secondary terminology** | Manufacturer describes advanced algorithms that automatically program AV synchrony. A trade-press search excerpt calls them AI, but primary documentation reviewed does not establish an AI/ML mechanism. |
| Micra VR2 | **AI not verified** | Leadless ventricular pacing, easier programming and improved longevity are documented. AV2-specific AV-synchrony algorithms must not be transferred to VR2. |
| AVEIR DR | **AI not verified** | Abbott describes synchronized pacing enabled by low-energy implant-to-implant electrical communication. i2i is a communication technology, not evidence of AI. |
| EMBLEM S-ICD | **AI not verified** | SMART Pass is explicitly described as a high-pass filter; rhythm-discrimination automation alone is insufficient to classify the system as AI. Current technical page principally concerns EMBLEM MRI A219, not every EMBLEM model/version. |
| EMPOWER leadless pacemaker | **AI not verified** | mSYNC transmits ATP requests from the S-ICD to the pacemaker. Communication, accelerometer rate response and automatic therapy coordination do not establish AI. |

**No onboard AI is verified for any of these six implants.** For BIOMONITOR, this is an affirmative location distinction for the described SmartECG implementation; for the others it is insufficient evidence, not a finding that their firmware is categorically non-AI.

## Decisive evidence

**AI01–AI02 — Manufacturer confirmation.** BIOTRONIK's [product documentation](https://www.biotronik.com/en-int/products/cardiac-rhythm-management/implantable-cardiac-monitor-systems/biomonitor-iv) explicitly states that SmartECG is supported by AI for AF detection. Its [12 June 2023 launch disclosure](https://www.biotronik.com/en-us/news/press-release/biotronik-announced-first-implant-of-new-implantable-cardiac-monitor-with-artificial-intelligence-targeting-efficiency-in-monitoring-for-cardiac-arrhythmias) narrows this in a footnote: “AI algorithm is applied only to AF detection.” Do not attribute all bradycardia, pause or tachycardia filtering to AI.

**AI03 — Execution location.** The [technical publication, DOI 10.3389/fcvm.2024.1343424](https://doi.org/10.3389/fcvm.2024.1343424), explicitly says SmartECG is implemented in HMSC and cannot be implemented in the ICM or interrogation programming device in the described system. This publication is BIOTRONIK-funded with manufacturer-linked authors; its analysis used BioMonitor IIIm recordings adapted to IV transmission limits. It supports architecture, not an independent prospective IV-only performance claim.

**AI04 — Micra terminology.** The [manufacturer's 1 May 2023 release](https://news.medtronic.com/2023-05-01-Medtronic-receives-FDA-approval-for-its-next-generation-Micra-leadless-pacing-systems) says “advanced algorithms that automatically program AV synchrony.” This is not sufficient to verify AI. The conflicting Cardiovascular Business wording was visible in search results, but direct access returned HTTP 403; it remains an uncorroborated secondary claim.

**AI05–AI06 — Communication and filtering.** [Abbott's technical product page](https://www.cardiovascular.abbott/us/en/hcp/products/cardiac-rhythm-management/pacemakers/aveir-dr-dual-chamber-leadless-pacemaker-system/why.html) describes conductive, subthreshold i2i pulses. [Boston Scientific's product documentation](https://www.bostonscientific.com/us/en/healthcare-professionals/products/defibrillators/emblem-mri-subcutaneous-implantable-defibrillator-s-icd-system/fp90000132.html) describes the SMART Pass high-pass filter and mSYNC ATP requests. Neither establishes AI. Boston Scientific's current page also labels EMPOWER/mCRM investigational in the US; this is manufacturer status language, not a fresh regulatory-database determination.

## How the files should now be read

- **Updated workbook** — opens on `AI verification`, with separate `AI evidence` and `AI methods` sheets. The original six sheets remain unchanged except for header comments pointing to the follow-up assessment.
- **Original CSVs** — retain the initial repository-only snapshot. Their `NOT_ESTABLISHED_IN_REVIEWED_OFFICIAL_RECORDS` status is historical and narrower than this expanded manufacturer-documentation review.
- **New verification CSV and evidence JSON** — contain six assessments and seven source entries, including exact supporting passages, URLs, source roles and qualifications. No paper-derived clinical performance values were added to the repository dataset.
- **Qinming** — remains outside the six verified entries because identity was unresolved. No defensible device-specific AI confirmation was established in this follow-up; repeating the review paper's own AI claims would be circular.

This is a targeted public-evidence check, not a source-code/firmware audit, comprehensive IFU review, or historical reconstruction of every product version. Current manufacturer pages can include later generations. Primary-page access failures included two Medtronic product pages (403), an Academy page without readable text, and an initially incorrect newsroom path (404); the correct dated manufacturer release was retrieved successfully. Absence of the terms AI/ML in a short document is not proof of no AI.
