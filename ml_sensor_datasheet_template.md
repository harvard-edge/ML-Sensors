# ML Sensor Datasheet
*(Editable Markdown template for documenting ML sensors)*

> This datasheet template follows the Findable, Accessible, Interoperable, and Reusable (FAIR) principles.  
> **How to use:** Duplicate this file, fill in each section, and update the version history when you revise the sensor, firmware, model, or evaluation results.

---

## Title Page

**Sensor Name:**  
**Short Description (1–2 sentences):**  

**Datasheet Version:**  
**Release Date:**  

**Authors / Maintainers:**  
**Affiliation(s):**  
**Contact Email:**  

**Repository URL:**  
**License:**  

**Related Paper / Citation:**  
- Paper:  
- BibTeX / DOI / URL:  

**Supported Hardware Variant(s):**  
- SKU / Part number:  
- Revision:  

**Supported Firmware / Software Version(s):**  
- Firmware version:  
- Driver version:  
- On-device runtime version (if applicable):  

**ML Model Identifier(s):**  
- Model name:  
- Model version / hash:  
- Training code commit (optional):  

**Version History**
| Version | Date | Changes | Updated By |
|---|---|---|---|
| 1.0.0 | YYYY-MM-DD | Initial release | Name |
| 1.0.1 | YYYY-MM-DD | Example: updated firmware version and re-ran end-to-end eval | Name |

---

## 1. Overview

### 1.1 Intended Use and Scope
**Primary use case(s):**  
**Out of scope / non intended use:**  
**Target deployment environments:** (indoor, outdoor, industrial, etc.)  
**Stakeholders:** (device integrators, end-users, auditors, regulators, etc.)

### 1.2 Sensor Outputs and Interface
**High-level outputs provided:** (e.g., person-present boolean, count, gesture label, confidence)  
**Output semantics:** (what the outputs mean, units, thresholds)  
**Update rate / sampling rate:**  
**Latency expectations:**  
**Confidence / uncertainty reporting:**  

### 1.3 Compliance and Certification
**Which international regulations and industry standards does the device conform to?**  
List applicable compliance regimes and standards. Include evidence and version scope.

- Data privacy regulations: (e.g., GDPR, etc.)  
- RF / communications regulations: (e.g., FCC, etc.)  
- Domain-specific regulations: (e.g., HIPAA, FDA, automotive safety, etc.)  
- Voluntary standards / best practices: (e.g., ISO 26262, etc.)  
- AI regulations (if relevant): (e.g., EU AI Act, etc.)  

**Certifications achieved:**  
- Certification body:  
- Certification name / ID:  
- Date obtained:  
- Scope (hardware/firmware/model versions covered):  
- Link to certificate or public record (if available):  

**Certification pathways (optional, future-facing):**  
How could this datasheet support third-party assurance or certification over time?  
- Re-certification triggers: (firmware update, model retraining, hardware revision)  
- Evidence package: (what data and tests would be required)

---

## 2. Model Characteristics

### 2.1 Software and Processing Flow
**Software flow diagram:** (insert image or link)  
**On-device pipeline summary:** (preprocessing, inference, postprocessing)  
**Key dependencies:** (runtime, libraries, hardware acceleration)  
**On-device resource usage:** (CPU/GPU/NPU, memory footprint)

### 2.2 Dataset Nutrition Label
**Training dataset(s):**  
- Dataset name(s):  
- Dataset version(s):  
- Data collection time period:  
- Data sources:  
- Labeling process:  
- Known limitations:  

**Evaluation dataset(s):**  
- Dataset name(s):  
- Dataset version(s):  
- Data collection time period:  
- Domain match to deployment: (high/medium/low)  

**Data governance:**  
- Consent and provenance:  
- Privacy considerations:  
- Data retention policy:  

**Bias and representativeness considerations:**  
- Demographic coverage (if applicable):  
- Known gaps:  
- Mitigations:  

### 2.3 IoT Security and Privacy Label
**Threat model summary:**  
**On-device data handling:** (stored? streamed? discarded?)  
**Encryption:** (at rest, in transit)  
**Authentication and authorization:**  
**Access control:**  
**Logging and audit trails:**  
**Privacy safeguards:** (on-device processing, minimization, redaction, etc.)  
**User controls:** (opt-out, data deletion, consent management)

### 2.4 Machine Learning Model Specifications
**Task:** (classification, detection, segmentation, etc.)  
**Model architecture:**  
**Input format:** (resolution, color space, sampling window)  
**Output format:** (labels, bounding boxes, confidence scores)  
**Training details:**  
- Training procedure summary:  
- Training compute (optional):  
- Hyperparameters (optional):  

**Model limitations:**  
- Failure modes:  
- Known edge cases:  
- Adversarial considerations (if applicable):

### 2.5 End-to-End Performance Analysis (Under Varying Conditions)
**What does “end-to-end” include for this sensor?**  
Define the full pipeline and versions covered.

**Evaluation version scope:**  
- Hardware revision:  
- Firmware/software version:  
- Model version:  
- Evaluation date:  

**Core metrics:**  
- Accuracy / F1 / mAP / etc.:  
- False positive rate:  
- False negative rate:  
- Calibration / confidence reliability (if applicable):  

**System metrics:**  
- End-to-end latency:  
- Throughput / FPS:  
- Power consumption:  
- Memory usage:  

**Environmental sensitivity:**  
Report performance under relevant environmental variables, for example:
- Lighting conditions:  
- Distance / range:  
- Motion blur / speed:  
- Occlusion:  
- Background clutter:  
- Temperature / humidity (if relevant):  

**Demographic performance and bias checks (if applicable):**  
- Groups evaluated:  
- Disparities observed:  
- Mitigations / caveats:  

**Performance over time (maintenance):**  
- Re-evaluation cadence: (e.g., quarterly, per firmware release)  
- Re-certification triggers: (what changes require re-evaluation)  
- Prior versions retained: (where to find them)

---

## 3. Hardware Characteristics

### 3.1 Hardware Details
**Device overview:**  
**Sensor modality:** (camera, IMU, microphone, etc.)  
**Compute subsystem:** (MCU/CPU/NPU, accelerator)  
**Memory:**  
**Power:** (supply requirements, typical draw)  
**Thermal constraints:**  
**Mechanical / form factor:**  

### 3.2 Communication Protocols
**I2C / SPI / UART / USB / Ethernet / Wi-Fi / BLE:**  
**Protocol details:** (addresses, packet format, timing constraints)  
**APIs / SDKs:** (links)  
**Reference drivers:** (links)

### 3.3 Device Diagrams
Insert or link diagrams:
- Block diagram:  
- Pinout:  
- Mechanical drawings:  
- Data flow diagram:

### 3.4 Bill of Materials (Optional)
| Component | Manufacturer | Part Number | Notes |
|---|---|---|---|
|  |  |  |  |

### 3.5 Environmental Impact (Optional but recommended)
**Materials and manufacturing notes:**  
**Power and energy usage notes:**  
**Estimated operational footprint (if available):**  
**Disposal / recyclability:**  
**Reporting standard used (if any):**  

### 3.6 Acronyms and Glossary
**Acronyms:**  
-  

**Glossary:**  
-  

---

## 4. User Study Materials (Optional)

### 4.1 Study Flyer
Link or embed.

### 4.2 Interest Form
Link or embed.

### 4.3 Consent Form
Link or embed.

---

## Appendix A. Change Impact Checklist (Recommended)
When updating this datasheet, check which aspects changed and require re-evaluation.

- [ ] Hardware revision changed
- [ ] Firmware / software changed
- [ ] Model retrained or updated
- [ ] Dataset changed
- [ ] Output semantics changed (thresholds, labels, calibration)
- [ ] End-to-end evaluation updated
- [ ] Privacy / security controls changed
- [ ] Certifications affected (notify certifier, re-certify)

---

## Appendix B. References
List key references, standards, and links:
-  
