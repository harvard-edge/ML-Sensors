# ML Sensor Datasheet Template
*(Fillable Markdown template for documenting ML sensors as versioned, auditable, reusable components)*


# Instructions for Use

1. Clone or download this template.  

2. Fill in all **[R] Required** fields and any **[C] Conditional** fields that apply.  

3. Tie performance results to specific hardware, firmware, model, dataset, and configuration versions.  

4. Submit updates via pull request so changes are reviewed and traceable.  

5. Tag each release with a version number and update the change log.  


---

**Legend:**

* **[R] Required** for a complete datasheet

* **[O] Optional** but strongly recommended

* **[C] Conditional** required depending on sensor and deployment

---

## Title Page

**[R] Sensor Name:**  

**[R] Sensor Type and Function:** (example: person detection, gesture recognition, occupancy, fall detection)  

**[R] Intended Use:** (what it is designed to do)  

**[R] Out of Scope or Non Intended Use:** (what it should not be used for)  

**[R] Version:**  

**[R] Release Date:**  

**[R] Last Updated:**  

**[R] Authors and Contributors:**  

**[R] Affiliation(s):**  

**[R] Maintainer:** (name or team responsible for updates)  

**[R] Contact Email:**  

**[R] Repository URL:**  

**[O] Issue Tracker URL:**  

**[R] License:**  

**[O] Cite This Datasheet:** (preferred citation text or link to CITATION file)  

**[R] Change Log:**

| Version | Date | Changes | Evaluations Updated | Approved By |
|--------|------|---------|--------------------|------------|
| 1.0.0  |      |         |                    |            |
|        |      |         |                    |            |

**[R] Artifact and Build Provenance (tie results to versions):**  

- Hardware revision:  

- Firmware version:  

- Model version or hash:  

- Training dataset version:  

- Evaluation dataset version:  

- Toolchain or runtime: (example: OS, framework version)  

**[O] Reproducibility Notes:** (how to reproduce the evaluation results, links to scripts, configs)  

> This datasheet follows the Findable, Accessible, Interoperable, and Reusable (FAIR) principles and is intended to be maintained as a versioned artifact.

---

## 1. Overview

**[R] One Sentence Summary:**  

**[R] Description:**  

**[R] Key Features:**  

**[R] Primary Use Cases:**  

**[R] Out of Scope or Non Intended Use Cases:**  

**[O] Stakeholders:** (developer, auditor, privacy officer, deployment operator, end user)  

**[C] Compliance and Certifications:**  

- Regulations and standards considered: (example: GDPR, FCC, ISO 27001, ISO 26262, HIPAA, EU AI Act)  

- Certification pathways considered: (example: third party safety assurance, UL style certification, security audit)  

- Current status: (not applicable, planned, in progress, certified)  

- Evidence links:  

**[R] Interface Summary (the sensor contract):**  

- Input modality: (camera, microphone, IMU, radar, multimodal)  

- Outputs exposed: (example: person present, gesture class, confidence, bounding box)  

- Output update rate:  

- Latency expectations:  

- Output validity conditions: (example: within 0.5 to 5 meters, indoor lighting only)  

- Tunable parameters exposed to users: (thresholds, smoothing, modes)  

**[R] Operating Envelope (supported and tested ranges):**

| Factor | Supported Range | Tested Range | Notes |
|-------|------------------|-------------|------|
| Lighting |  |  |  |
| Distance |  |  |  |
| Angle / FOV |  |  |  |
| Motion / speed |  |  |  |
| Occlusion |  |  |  |
| Temperature |  |  |  |
| Other |  |  |  |

**[R] Safety, Misuse, and Harm Considerations:**  

- Foreseeable misuse:  

- Potential harms:  

- Mitigations or guardrails:  

- Human oversight expectations: (if any)  

---

## 2. System and Software Characteristics

**[R] System Block Diagram or Software Flow Diagram:** (link or embedded image)  

**[R] Pipeline Stages:** (sensing, preprocessing, inference, postprocessing, output interface)  

**[C] On Device vs Cloud Components:** (what runs where)  

**[R] Runtime Dependencies:** (frameworks, libraries, OS)  

**[R] Update Mechanism:** (OTA, manual, none)  

**[R] Versioning Policy:** (what changes require a new datasheet version)  

**[R] Default Configuration (used for reported metrics):**  

- Frame rate or sampling rate:  

- Resolution or sampling parameters:  

- Preprocessing settings: (crop, normalization, filtering)  

- Confidence threshold:  

- Postprocessing: (smoothing, tracking)  

- Quantization mode: (if applicable)  

**[O] Configurability:**  

- Tunable parameters and recommended ranges:  

- Tradeoffs: (accuracy vs latency vs power)  

---

## 3. Data and Model Characteristics

### 3.1 Evaluation Data (for reported results)

**[R] Evaluation Dataset Name and Version:**  

**[R] Source and Access:** (public link, internal, restricted)  

**[R] License and Usage Constraints:**  

**[R] Ground Truth Method:** (human labeling, sensor fusion, annotation protocol)  

**[R] Coverage Summary:** (conditions represented, demographics if applicable)  

**[R] Known Limitations:**  

### 3.2 Training Data (if different from evaluation data)

**[C] Training Dataset Name and Version:**  

**[C] Source and Access:**  

**[C] License and Usage Constraints:**  

**[C] Collection Context:** (where, when, how)  

**[C] Labeling Process:**  

**[C] Known Biases and Limitations:**  

### 3.3 Model Documentation

**[R] Model Task:**  

**[R] Model Architecture and Size:** (high level description)  

**[R] Model Version or Hash:**  

**[C] Training Procedure Summary:** (if you trained it)  

**[O] Compute Used for Training:** (if known)  

**[R] Intended Use and Limitations:** (model card style short summary)  

---

## 4. Security and Privacy Labeling

**[R] Data Handling Summary:**  

- Does it capture potentially identifiable data: (yes, no, depends)  

- Where processing occurs: (on device, cloud, hybrid)  

- Data stored on device: (what, how long)  

- Data transmitted off device: (what, when)  

- Data retention policy:  

- Consent and notice expectations: (where applicable)  

**[R] Security Controls:**  

- Encryption in transit:  

- Encryption at rest:  

- Authentication and access control:  

- Logging and audit trails:  

**[R] Vulnerability Handling and Updates:**  

- Security contact:  

- Disclosure process:  

- Patch mechanism and timelines:  

- Supported lifetime:  

**[O] IoT Security and Privacy Label:** (link or table if you maintain a standardized label)  

---

## 5. End to End Performance Characterization

This section reports system level performance of the complete ML sensor as deployed. All results must be tied to the specific versions listed on the title page.

**[R] Evaluation Setup:**  

- Hardware revision:  

- Firmware version:  

- Model version or hash:  

- Evaluation dataset version:  

- Configuration used: (link to config file or list key parameters)  

- Environment description: (where tests were run)  

**[R] Core Metrics:**  

- Accuracy metrics: (example: precision, recall, F1, mAP, AUROC)  

- Latency: (p50, p95)  

- Throughput or update rate:  

- Power consumption: (idle, active, peak)  

- Memory footprint:  

**[R] Environmental Sensitivity Results:**  

- Lighting:  

- Distance and angle:  

- Occlusion and motion:  

- Temperature or other relevant factors:  

**[C] Demographic and Fairness Analysis:**  

- Demographic slices evaluated:  

- Observed disparities:  

- Mitigations or caveats:  

- Not evaluated and why:  

**[R] Failure Modes and Known Limitations:**  

- Common failure cases:  

- Conditions that invalidate outputs:  

- Recommended fallback behavior:  

**[O] Monitoring, Drift, and Diagnostics:**  

- Signals to monitor in deployment:  

- Drift detection approach:  

- Triggers for reevaluation and datasheet update:  

---

## 6. Hardware Characteristics

**[R] Hardware Overview:**  

**[R] Hardware Revision:**  

**[R] Compute Components:** (MCU, GPU, NPU, accelerator)  

**[R] Sensor Components:** (camera module, microphone, IMU, radar)  

**[R] Memory and Storage:**  

**[R] Power Requirements:** (voltage, current, battery considerations)  

**[R] Thermal Constraints:**  

**[O] Mechanical and Mounting Notes:**  

**[C] Interfaces and Protocols:**  

- I2C details: (if applicable)  

- SPI, UART, USB, WiFi, BLE:  

- Pinout or connector details:  

**[O] Device Diagrams:** (links or embedded images)  

**[O] Bill of Materials:** (major components, optional cost notes)  

---

## 7. Environmental Impact

**[R] Operational Energy Use:** (tie back to power metrics)  

**[O] Manufacturing and Materials Notes:** (where known)  

**[O] Packaging and Shipping Notes:**  

**[R] Model Lifecycle Impact:** (retraining frequency, update cadence)  

**[O] End of Life Considerations:** (recycling, disposal guidance)  

---

## 8. Maintenance and Release Process

**[R] What Requires a Datasheet Update:**  

- Firmware change  

- Model retraining or fine tuning  

- Training or evaluation dataset update  

- Hardware revision  

- Interface change  

- Security patch  

**[R] Recommended Evaluation Cadence:** (example: every release, quarterly, after any update)  

**[O] Backward Compatibility Notes:**  

**[O] Deprecation Policy:**  

---

## 9. Acronyms and Glossary

**[O] Acronyms:**  

**[O] Glossary:**  

---

## 10. User Study Materials
*(Include only if applicable. Link to forms rather than embedding sensitive content.)*

**[C] Study Flyer:**  

**[C] Interest Form:**  

**[C] Consent Form:**  

**[C] IRB or Ethics Reference:**  
