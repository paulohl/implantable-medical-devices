# AI mechanism verification

**Paper:** Leocadio (2024), DOI 10.5121/ijcsit.2024.02101  
**Checked:** 28 October 2026. Six device-level assessments, including separate Micra AV2 and VR2 assessments. Original 22 corpus passages preserved; 13 new mechanism excerpts added in separate workbook sheets.

## Finding that changes the earlier assessment

**SmartECG’s AI is verified as remote-platform software, not AI executing inside the implanted monitor.** The initial pilot left this location unconfirmed. A primary research article published on 23 January 2024 now resolves it directly:

> “The SmartECG algorithm is implemented in the remote monitoring platform because it cannot be implemented in the ICM or in the programming device used to interrogate the ICM during a follow-up visit.”

— Bisignani et al., Discussion, “Remote vs. in-office follow-up” [V01; M03].

This supports describing an **AI-enabled implantable-monitoring system**, not an implant containing an autonomous AI treatment controller. The source predates the paper’s nominal February 2024 publication but postdates the 16 January retrieval dates visible in its references. It is newly added evidence, not a source the paper already cited.

## Device-level results

### BIOMONITOR IV / SmartECG — AI function and location verified; architecture undisclosed

**Signal path:** the implanted monitor records subcutaneous ECGs → daily remote transmission to the Home Monitoring Service Center → SmartECG signal processing and AI-assisted AF classification → episode labels for clinical review.

The article identifies QRS signal processing and limits the additional AI function to AF events. It explicitly excludes patients whose ECGs had contributed to AI training from its evaluation cohort [M01–M05]. This establishes data-trained AI more firmly than marketing terminology alone. It does **not** disclose enough to verify a neural-network architecture, model weights, the full training corpus, or continuous online learning. There is no basis here for claiming autonomous adaptive therapy.

**Validation boundary:** the analysis included 368 patients and 61,517 ECGs; it used BioMonitor IIIm recordings adjusted to approximate IV transmissions. SmartECG was assessed at the “balanced” setting, whereas the 2023 release’s 86% claim used “Very Specific.” The reported 42.8% filtering of all ECGs and estimated workload reduction are not the same endpoint as 86% fewer false positives. Workload reduction assumes filtered ECGs are ignored; it is not a randomized measured before/after time saving or improved patient outcome. Funding was from Biotronik, and an author was a Biotronik employee. Training-patient exclusion supports patient separation, not independent replication.

### Micra AV2 — automatic sensing/control verified; ML not established

The manufacturer brochure describes accelerometer-based mechanical atrial sensing. Atrial Sensing Setup sets A3/A4 thresholds and sensing-window parameters. Auto+ sets its A3 threshold relative to measured A3/A7 amplitudes; Auto PVAB adjusts atrial blanking based on ventricular rate [V02, pp. 6–13; M06–M08].

These are documented sensor-driven control rules implemented by the implanted pacemaker. They do not establish a trained classifier or neural network. “Automatic,” patient-specific adjustment and “smarter algorithms” are insufficient evidence of ML. The available description does not prove every proprietary firmware component is non-AI.

### Micra VR2 — distinguish rate response from AV2 atrial sensing

The brochure’s specification table lists accelerometer-based rate response for VR2 but mechanical atrial sensing as “N/A” [V02, p. 4; page image checked]. Do not transfer AV2’s mechanical-atrial-sensing and AV-synchrony algorithms to VR2. AI/ML is not established by the examined documentation.

### AVEIR DR i2i — electrical communication verified; ML not established

Abbott’s December 2023 chief-engineer interview describes bidirectional, beat-to-beat **conducted electrical signaling**, with low-frequency wake-up pulses followed by digital messages. Signal strength can be adjusted using diagnostics during programming sessions [V03; M09–M10].

That is a communication protocol between two implants. Customization and communication-loss safeguards do not demonstrate a learned model. The source provides no training procedure or ML architecture. Describe the documented feature as implant-to-implant coordination rather than AI integration.

### EMBLEM S-ICD + EMPOWER — command-to-pacing mechanism verified; ML not established

The public MODULAR ATP protocol specifies fixed-threshold sensing with programmable threshold and accelerometer-based rate response for EMPOWER. Its communication test sends a command from the S-ICD that triggers an ATP response in EMPOWER [V04, pp. 124 and 130; M11–M12].

This verifies the command/therapy path, not a learning mechanism. It does not characterize every S-ICD detection algorithm or show that all firmware is non-AI. EMPOWER is intracardiac; the S-ICD’s extrathoracic position does not apply to the entire system. The protocol is Version I, 29 April 2022; its first public-posting date was not established.

### Qinming8631 DR — AI claim unresolved; trial does not specify it

The 2016 randomized trial evaluates dual-chamber pacing, including rate response [V05; M13]. It does not establish a learned model or describe the internal controller in enough detail to classify its exact sensing algorithm. The defensible result is **AI integration unverified**, not “confirmed no AI.” QM7211 remains a ventricular electrode lead, not the pacemaker model.

## Sources and access

- **V01 — added external primary source; also verified by CiteRight:** Bisignani et al. (2024), *Frontiers in Cardiovascular Medicine* 11:1343424. [DOI](https://doi.org/10.3389/fcvm.2024.1343424). Full HTML read; CC BY. Exact device-specific support for AI scope, training separation and computation location.
- **V02 — added manufacturer technical source:** Medtronic, *Micra leadless pacemakers*, UC202002938e EN 05/2023. [PDF mirror](https://pdfs.semanticscholar.org/57d9/24ea3b36b976d9deeb0442f3d027ac70fc8d.pdf). Official-host download returned HTTP 403; the mirrored manufacturer PDF was read directly and dated from its footer. Copyrighted.
- **V03 — added manufacturer engineering source:** Abbott Cardiac Rhythm Management, 14 December 2023. [Engineer interview](https://www.cardiovascular.abbott/us/en/hcp/products/cardiac-rhythm-management/blog/unveiling-the-i2i-communication-technology-in-aveir-dr.html). Copyrighted; live full text read.
- **V04 — added primary protocol:** Boston Scientific, *MODULAR ATP Clinical Investigation Plan*, Version I, 29 April 2022, NCT04798768. [Public registry PDF](https://cdn.clinicaltrials.gov/large-docs/68/NCT04798768/Prot_000.pdf). Selected device and communication sections read. Although publicly posted, it is marked confidential and restricts copying; only short attributed excerpts retained, not the full document redistributed.
- **V05 — existing workspace corpus source S03, rechecked:** Xiang et al. (2016), *Chinese Medical Journal* 129:2659–2665. [DOI](https://doi.org/10.4103/0366-6999.193443). Full open publisher text read; exact reuse licence unresolved.

CiteRight report 1673502 independently surfaced V01 as the exact-match reference. Four other suggestions were general reviews/background, not device-specific mechanism verification, and were excluded for that reason. No source code, firmware binary or proprietary model weights were inspected. A 2025 Micra paper appeared in search but its full text was inaccessible; no conclusions here depend on it. Search availability was limited, so this is a targeted verification rather than an exhaustive search proving absence of AI.

## How to use the workbook

The new first sheet, **AI verification**, has verdicts and safe descriptions. **Mechanism passages** preserves 13 quotations with locators, interpretations and dates; **Mechanism sources** identifies their provenance and rights. Original **Passages**, **Sources** and **Codebook** sheets remain unchanged as the initial pilot record. Mechanism codes are a separate extension: LOCUS_CONFIRMED, AI_EXPLICIT, TRAINING_EVIDENCE, VALIDATION_BOUNDARY, CONTROL_RULE, AUTOMATION, COMMUNICATION, PROGRAMMING and EVIDENCE_LIMIT are descriptive labels, not estimates of algorithm quality.

The initial synthesis memo remains a historical pilot deliverable. This report supersedes its uncertainty about SmartECG’s computation location and adds the January 2024 primary validation evidence. No manuscript text has been edited.
