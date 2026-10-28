# Proposed corrections to Sections 4–5

**Manuscript:** Leocadio (2024), DOI 10.5121/ijcsit.2024.02101  
**Draft prepared:** 28 October 2026  
**Basis:** Original manuscript, the workbook’s AI verification and Clinical trials sheets, and their linked primary-source excerpts. This is a proposed replacement, not an edit to the published PDF.

## Author notes — not for insertion

- The replacement retains the manuscript’s existing numbering beginning at 4.4; it does not invent missing Sections 4.1–4.3.
- The main text uses evidence published before the February 2024 issue. Bisignani et al. appeared on 23 January 2024, after the manuscript’s January 16 retrieval dates. Update the documented search/retrieval boundary if adding it; do not imply the original submission cited it.
- The optional MODULAR ATP paragraph is a later update, not a correction based on evidence available in February 2024.
- Existing citations are retained where their supported claims remain. Unsupported AI labels and misattributed citations are not retained merely to preserve the reference list. Add the primary and technical references identified below before submission.

---

## Replacement text begins

## 4. Case Studies of Implantable Cardiac Devices and Associated Computational Functions

The following case studies examine implantable cardiac devices with different monitoring and therapeutic functions. Automatic adjustment, programmable control and implant-to-implant communication should not be classified as AI without evidence of a trained model. The location of computation also matters. SmartECG associated with BIOTRONIK’s BIOMONITOR IV performs AI-assisted atrial fibrillation classification in the remote Home Monitoring Service Center, rather than within the implant or programmer (Bisignani et al., 2024). It is therefore an AI-enabled monitoring system, not an example of implant-resident AI controlling treatment.

### 4.4. Medtronic’s Micra AV2 and Micra VR2 Leadless Pacemakers

#### 4.4.1. Description

Micra AV2 and Micra VR2 are leadless ventricular pacemakers used to treat bradycardia (Wainscot Media, 2023). Micra AV2 uses an accelerometer to detect mechanical atrial activity and support atrioventricular (AV) synchrony. Micra VR2 provides rate-responsive ventricular pacing but does not have AV2’s mechanical atrial-sensing capability. Manufacturer documentation describes automatic sensing and control functions; it does not establish that these functions use machine learning (Medtronic, 2023).

#### 4.4.2. Applications and Benefits

Both devices provide pacing without transvenous leads or a subcutaneous generator pocket. AV2 additionally supports AV-synchronous ventricular pacing through mechanical atrial sensing. These features should be described as pacing capabilities rather than evidence that AI improves patient outcomes.

#### 4.4.3. Strengths and Potential Weaknesses

The leadless design avoids the need for a transvenous pacing lead and generator pocket. Implantation nevertheless carries risks, including cardiac injury, pericardial effusion or tamponade, and failure to deliver effective therapy. Evidence from earlier Micra systems provides context but should not be treated as direct validation of AV2 or VR2. In the Medtronic-sponsored MARVEL 2 study, the primary efficacy analysis included 40 patients and assessed an accelerometer-based algorithm for up to five hours (Steinwender et al., 2020). AccelAV was a single-arm study of Micra AV; its primary subgroup of 54 patients had mean resting AV synchrony of 85.4% and ambulatory synchrony of 74.8% at one month (Chinitz et al., 2023). Neither study isolates an AI effect.

#### 4.4.4. Distinguishing Features

Manufacturer-reported projected median battery longevity is approximately 16 years for AV2 and 17 years for VR2 (Wainscot Media, 2023). These are projections, not observed durations of clinical follow-up or guarantees for individual patients. AV2’s automatic atrial-sensing adjustments should not be assigned to VR2. Remote monitoring and easier programming are operational features, not evidence of machine learning.

### 4.5. Qinming8631 DR Dual-Chamber Pacemaker

#### 4.5.1. Description

Qinming8631 DR is a programmable, dual-chamber, rate-responsive pacemaker evaluated for bradycardia treatment (Prutchi, Chinese Pacemakers by Qinming Originated in Delaware, 2023; Xiang et al., 2016). It should not be confused with QM7211, which is a ventricular electrode lead. The examined clinical report does not establish an AI or machine-learning component.

#### 4.5.2. Applications and Benefits

The device provides dual-chamber pacing with rate response. Its clinical evidence concerns pacing performance rather than AI-assisted diagnosis or autonomous learning. In a randomized multicenter trial, 225 patients received Qinming8631 DR or a Talos DR comparator; the authors reported noninferiority for effective pacing at six months (Xiang et al., 2016).

#### 4.5.3. Strengths and Potential Weaknesses

The randomized comparison provides evidence beyond a manufacturer description. However, six-month follow-up does not establish long-term durability. The per-protocol completion sets comprised 87 of 113 Qinming recipients and 86 of 112 comparator recipients. The article reports no financial sponsorship and describes third-party data analysis, but these disclosures do not independently verify all aspects of study governance (Xiang et al., 2016).

#### 4.5.4. Distinguishing Features

Programmable dual-chamber pacing and rate response are the documented functions relevant to this comparison. Claims about a trained model, its architecture or learning behavior cannot be made from the examined evidence.

### 4.6. Boston Scientific’s EMBLEM S-ICD and EMPOWER Leadless Pacemaker

#### 4.6.1. Description

The modular system combines the EMBLEM subcutaneous implantable cardioverter-defibrillator with the EMPOWER intracardiac leadless pacemaker (Prutchi, Boston Scientific Starts Trial of EMBLEM™ S-ICD with EMPOWER™ Leadless Pacemaker, 2023). The S-ICD provides defibrillation and can transmit a command requesting antitachycardia pacing from EMPOWER. The documented command-and-response mechanism does not establish machine learning (Boston Scientific, 2022).

#### 4.6.2. Applications and Benefits

The system was being investigated as a means of combining defibrillation with pacing while avoiding transvenous leads. The components have different functions: EMPOWER provides pacing, whereas the S-ICD delivers defibrillation. The combined system should therefore not be described as unable to defibrillate.

#### 4.6.3. Strengths and Potential Weaknesses

Randomized evidence supports selected benefits of the S-ICD component, not the complete modular system. PRAETORIAN established noninferiority to transvenous ICDs for a composite of device-related complications and inappropriate shocks in patients without a pacing indication (Knops et al., 2020). ATLAS reported major lead-related complications in 0.4% of S-ICD recipients versus 4.8% of transvenous ICD recipients, but was underpowered for differences in shock outcomes (Healey et al., 2022). Both trials were academically led and funded by Boston Scientific. Their results neither establish an AI benefit nor validate all risks of adding EMPOWER.

#### 4.6.4. Distinguishing Features

The S-ICD generator and lead are extrathoracic; EMPOWER is implanted inside the heart. Consequently, a description of the device as never touching the heart applies only to the S-ICD component. The distinguishing feature of the combined system is coordinated defibrillation and leadless pacing, not verified AI integration.

### 4.7. Abbott’s AVEIR DR and i2i Communication

#### 4.7.1. Overview

AVEIR DR is Abbott’s dual-chamber leadless pacing system. Its atrial and ventricular implants exchange conducted electrical signals through i2i communication to coordinate pacing. The manufacturer’s engineering description documents bidirectional communication rather than a trained predictive model (Abbott, 2023b).

#### 4.7.2. Clinical Evidence and Limitations

The Abbott-funded prospective, multicenter, single-group study evaluated 300 patients. Implantation succeeded in 295 patients (98.3%). At 90 days, 271 patients (90.3%) were free from device- or procedure-related serious adverse events; 35 such events occurred in 29 patients. At least 70% AV synchrony was achieved in 97.3% of patients (Knops et al., 2023). The latter figure is a proportion meeting a synchrony threshold, not mean synchrony of 97.3%. These results support short-term system performance against prespecified goals, but the absence of a concurrent control limits comparative conclusions. The study did not isolate an AI contribution.

## 5. Comparative Analysis

The devices differ in clinical purpose and computational mechanism. Their comparison therefore requires separate consideration of monitoring, pacing and defibrillation. Evidence of device performance should also be distinguished from evidence that an AI component improves that performance.

### 5.1. Functionalities

BIOMONITOR IV records subcutaneous ECGs for remote review, with SmartECG providing remote-platform AI-assisted AF classification (Bisignani et al., 2024). Micra AV2 supports ventricular pacing synchronized to mechanically sensed atrial activity, whereas Micra VR2 provides rate-responsive ventricular pacing without that atrial-sensing function (Medtronic, 2023). Qinming8631 DR provides dual-chamber rate-responsive pacing; QM7211 is a lead rather than the pacemaker (Xiang et al., 2016; Prutchi, Chinese Pacemakers by Qinming Originated in Delaware, 2023). EMBLEM and EMPOWER combine defibrillation with commanded pacing (Boston Scientific, 2022). AVEIR DR coordinates atrial and ventricular pacing through implant-to-implant electrical communication (Abbott, 2023b).

Among these examined functions, SmartECG has explicit evidence of data-trained AI. The other descriptions establish automatic control or communication without establishing machine learning. Incomplete proprietary documentation does not, however, prove that every undisclosed component is non-AI.

### 5.2. Applications and Clinical Evidence

These systems are not interchangeable treatments. An implantable monitor records arrhythmias but does not provide pacing or defibrillation. Pacemakers treat bradycardia, while ICD systems address potentially dangerous ventricular arrhythmias. Clinical findings must therefore be interpreted within the population and indication studied.

PRAETORIAN and ATLAS provide randomized evidence concerning S-ICD comparisons, not AI (Knops et al., 2020; Healey et al., 2022). The Qinming trial evaluates pacing noninferiority (Xiang et al., 2016). MARVEL 2 and AccelAV concern predecessor Micra technology, and the AVEIR study evaluates a single-group dual-chamber system (Steinwender et al., 2020; Chinitz et al., 2023; Knops et al., 2023). None of these included trials isolates the clinical effect of AI. Academic leadership, manufacturer funding and independent event adjudication should be reported separately rather than reduced to a single claim of independence.

### 5.3. Distinguishing Features and Evidence Limits

SmartECG’s remote AI classification differs from implant-resident pacing control. Its January 2024 evaluation used 61,517 ECGs from 368 patients and estimated review-workload reduction using recordings adapted from BioMonitor IIIm workflows. The analysis was industry-funded and did not establish improved patient outcomes (Bisignani et al., 2024).

For Micra AV2 and VR2, projected battery longevity should not be treated as observed survival. For EMBLEM and EMPOWER, component location and function must remain distinct. For AVEIR, implantation success, freedom from serious adverse events and achievement of a synchrony threshold are different endpoints. These heterogeneous results do not support a numerical ranking of overall device effectiveness or AI benefit. The comparison instead identifies which functions are documented and where stronger clinical evidence is required.

## Replacement text ends

---

## Optional later-update paragraph — exclude from a historically bounded February 2024 correction

Subsequent MODULAR ATP results, first published on May 18, 2024, provide direct evidence for the combined EMBLEM–EMPOWER system. The study enrolled 293 patients, with 162 in the six-month endpoint cohort and 151 completing the six-month visit. Freedom from major leadless-pacemaker complications was 97.5%, and communication succeeded in 98.8% of tests. The single-group study had independent event adjudication but sponsor-performed outcome analyses; it did not isolate an AI effect (Knops et al., 2024).

## Correction map — editorial guidance, not replacement prose

| Location | Correction | Workbook evidence |
|---|---|---|
| Section 4 title and introduction | Do not classify all cases as verified AI-integrated implants. Locate SmartECG processing outside the implant. | AI verification; V01, M01–M05 |
| 4.4.1 and 5.1 | Replace unsupported advanced-AI labels with documented sensing/control functions. AV is atrioventricular. Separate AV2 from VR2. | V02, M06–M08; V02 p.4 specification table |
| 4.4.3 | Identify predecessor models and short/subgroup endpoints; do not imply AI causality. | T04–T05 |
| 4.4.4 and 5.3 | Replace inconsistent 8–13/12-year statements with clearly attributed projected medians near 16/17 years. Avoid lifetime guarantees. | Original pilot Micra evidence; manufacturer technical source |
| 4.5 and 5.1–5.3 | Use Qinming8631 DR for the pacemaker. QM7211 is a ventricular lead. Replace unsupported AI characterization. | Existing S03/V05; T03 |
| 4.6.2–4.6.4 | Attribute defibrillation to EMBLEM and pacing to EMPOWER. Extrathoracic position does not describe EMPOWER. Avoid claims that all procedural risk is eliminated. | V04, M11–M12; T01–T02 |
| 4.7.1 | AVEIR is an Abbott system, not a manufacturer. Remove the unrelated BACKBEAT IDE citation. | V03, M09–M10; T06 |
| 4.7.2 | Separate 98.3% implantation success, 90.3% 90-day safety, and 97.3% meeting a ≥70% synchrony threshold. Include serious events. | T06; C13–C15 |
| Section 5 | Distinguish clinical indications and evidence designs rather than ranking heterogeneous endpoints. Qualify independence and AI-specific inference. | All six device assessments and T01–T07 |

## Reference additions and source crosswalk

Use the journal’s reference style. Existing reference-list entries can remain where still cited elsewhere. “Abbott, 2023b” is a provisional disambiguation for the engineering article, distinct from the manuscript’s existing Abbott press release; reconcile the a/b labels across the full manuscript.

- **Bisignani et al. (2024), V01:** *Implantable cardiac monitors: artificial intelligence and signal processing reduce remote ECG review workload and preserve arrhythmia detection sensitivity.* Frontiers in Cardiovascular Medicine 11:1343424. DOI: https://doi.org/10.3389/fcvm.2024.1343424. Added primary mechanism/validation source; full HTML examined.
- **Medtronic (2023), V02:** *Micra leadless pacemakers*, UC202002938e EN, 05/2023. Manufacturer technical brochure, particularly pp.4 and 6–13. Examined copy: https://pdfs.semanticscholar.org/57d9/24ea3b36b976d9deeb0442f3d027ac70fc8d.pdf.
- **Boston Scientific (2022), V04:** *MODULAR ATP Clinical Investigation Plan*, Version I, 29 April 2022, NCT04798768; selected device/communication sections. https://cdn.clinicaltrials.gov/large-docs/68/NCT04798768/Prot_000.pdf. Publicly posted protocol, not a clinical results paper; document bears redistribution restrictions.
- **Abbott (2023b), V03:** Engineering interview on AVEIR DR i2i communication, 14 December 2023. https://www.cardiovascular.abbott/us/en/hcp/products/cardiac-rhythm-management/blog/unveiling-the-i2i-communication-technology-in-aveir-dr.html. Manufacturer engineering source, not independent clinical validation.
- **Xiang et al. (2016), T03 / S03 / V05:** Qinming8631 DR randomized comparison, Chinese Medical Journal 129:2659–2665. DOI: https://doi.org/10.4103/0366-6999.193443. Existing manuscript/corpus reference; full article examined.
- **Knops et al. (2020), T01:** *Subcutaneous or Transvenous Defibrillator Therapy.* New England Journal of Medicine. DOI: https://doi.org/10.1056/NEJMoa1915932. PRAETORIAN; full primary article examined.
- **Healey et al. (2022), T02:** ATLAS randomized S-ICD versus transvenous ICD outcome report. Annals of Internal Medicine. DOI: https://doi.org/10.7326/M22-1566. Primary abstract and investigator materials examined; full journal article not audited.
- **Steinwender et al. (2020), T04:** *Atrioventricular Synchronous Pacing Using a Leadless Ventricular Pacemaker: Results From the MARVEL 2 Study.* JACC: Clinical Electrophysiology. DOI: https://doi.org/10.1016/j.jacep.2019.10.017. Online publication 2019; primary abstract and registry examined.
- **Chinitz et al. (2023), T05:** *Ambulatory atrioventricular synchronous pacing over time using a leadless ventricular pacemaker: Primary results from the AccelAV study.* Heart Rhythm. DOI: https://doi.org/10.1016/j.hrthm.2022.08.033. Online publication 2022; primary abstract and registry examined.
- **Knops et al. (2023), T06:** *A Dual-Chamber Leadless Pacemaker.* New England Journal of Medicine. DOI: https://doi.org/10.1056/NEJMoa2300080. Primary abstract and registry examined; full article/supplement not audited.
- **Knops et al. (2024), T07 — optional later update only:** *A Modular Communicative Leadless Pacing–Defibrillator System.* New England Journal of Medicine. DOI: https://doi.org/10.1056/NEJMoa2401807. First online publication 18 May 2024; full primary article examined.

## Scope and submission checks

This draft does not update Sections 1–3 or 6–8. In particular, Section 3.2’s AI-location description and Section 8.2’s QM7211 identification and blanket AI framing need corresponding changes if these replacements are adopted. Those inconsistencies are flagged, not silently edited. Retain the distinction between public accessibility and open licensing when reusing quoted source material. No new literature search or full-supplement audit was performed for this drafting step.
