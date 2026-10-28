# Implantable devices: what the primary sources actually support

**Evidence pilot for Paulo H. Leocadio’s 2024 paper**  
DOI: 10.5121/ijcsit.2024.02101 · Completed 28 October 2026

## Bottom line

The sampled primary sources support advances in cardiac-device engineering and short-term performance, but they do not support treating every named device as a demonstrated AI application. **BIOMONITOR IV is the only one of the five device families whose sampled source explicitly identifies AI.** Its AI function is limited to atrial-fibrillation detection. That is a finding about these documents—not proof that the other devices lack AI.

This distinction would make the paper’s comparison more defensible: separate **documented AI**, **automatic pacing**, and **device-to-device communication** before comparing benefits.

## Argument and evidence needed

The paper argues that AI integration across manufacturers improves monitoring and personalized treatment while creating adoption challenges (§§3–8). Its empirical examples are predominantly cardiac, despite the wider implantable-device framing. It is a narrative analysis: p. 15 states, “No data were used in writing this paper, other than publicly available citations.” There is no original patient dataset or specified systematic search to reproduce.

Accordingly, this task builds a new, small claim-evidence corpus: **22 passages from six primary documents**, covering all five cardiac-device families plus cybersecurity law. The scheme follows the paper’s distinctions—function, performance, regulation and adoption—but adds identity checks and inference limits. No synthetic observations were used.

A stronger test of the central AI argument needs device-specific descriptions of the learned model and where it runs; public validation against a stated comparator; patient outcomes or workflow effects attributable to AI; and adoption measures such as eligible-patient uptake, cost or clinician use. Approval, trial enrollment and technical capability do not establish uptake.

## Findings across the cases

| Case | What is supported | Boundary exposed by coding |
|---|---|---|
| BIOMONITOR IV | Manufacturer claims 86% fewer false-positive detections while preserving 98% of true episodes (P04). | AI applies only to AF detection (P01). The comparator is performance without SmartECG (P03); the cited basis is data on file. The filtering setting is in the Home Monitoring Service Center (P02), so implant-resident AI is not established. |
| Micra AV2 / VR2 | Automatic AV synchrony in AV2; projected median battery life nearly 16/17 years (P05–P06). | Automatic algorithms do not establish machine learning. Longevity is projected, not observed over 16–17 years. AV2’s synchrony feature should not be assigned to VR2. |
| Qinming8631 DR | A randomized, single-blind noninferiority trial at 14 Chinese sites; 225 randomized; six-month follow-up (P08–P11). | This tests pacing performance, not an AI intervention. **QM7211 is a ventricular electrode lead**, not the pacemaker model used in §5 (P09). |
| EMBLEM / EMPOWER | A planned nonrandomized trial of modular communication and pacing (P12–P15). | The 2021 release calls EMPOWER investigational, not for sale. “Without touching the heart” describes the S-ICD component, not the combined system. Communication is not itself AI. |
| AVEIR DR i2i | Sponsor reports 300 people at 55 centers, 98.3% implant success and >97% meeting an AV-synchrony endpoint (P16–P19). | The three-month, single-arm study does not isolate an AI effect. The percentage of people meeting the endpoint is not the same measure as average AV synchrony across postures. |

The statute supplies direct support for the paper’s security/regulatory discussion: qualifying cyber-device submissions require a vulnerability-management plan and software bill of materials (P20–P22). These obligations are not AI-specific and do not establish compliance by any named product. Internet connectivity is only one of the statutory definition’s three conditions.

## Highest-value changes to the analysis

1. **Reclassify mechanisms before comparing devices.** Retain BIOMONITOR’s explicit AF-detection AI; mark AI/ML status as unverified for the other sampled cases pending technical documentation. Do not interpret that uncertainty as absence.
2. **Correct component attribution.** Replace the QM7211 pacemaker label with Qinming8631 DR; distinguish S-ICD placement from EMPOWER’s intracardiac component. Resolve Micra’s conflicting longevity figures by labeling the source’s 16/17-year medians as projections.
3. **Separate evidence stages and denominators.** Keep diagnostic filtering, implant success, pacing endpoints and battery projections in different columns. Add a separate adoption evidence column rather than inferring uptake from approval or prospective trials.

## Limits and reuse

This is a purposive, single-coder pilot, not a systematic review, meta-analysis or device ranking. Four documents are manufacturer/sponsor releases, one is an original randomized trial and one is primary legislation. Passages within a document are not independent studies. Sources predate the paper, but were retrieved from current web copies; no historical snapshot was authenticated. Boston’s investigational status is recorded at its December 2021 source date, not asserted as February 2024 status.

Eighteen excerpts passed automated substring checks; four Qinming excerpts were verified against the full publisher text because direct re-fetching did not expose the same article text. PMC/PubMed returned browser checks. Quotes are verbatim with HTML entities decoded and whitespace normalized; coding and interpretations are separate fields.

**Access is not a reuse licence.** The four corporate releases are openly readable but copyrighted, with no open reuse licence verified. The trial is marked Open, but its exact licence was not verified. The quoted US statute is public-domain text. Short attributed excerpts are retained; do not redistribute the collection as wholly CC-licensed content. Full definitions, source metadata and rights are in the accompanying protocol and workbook.
