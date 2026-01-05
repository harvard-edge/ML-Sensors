# Machine Learning Sensors (ML Sensors)

This repository contains resources for the **ML sensor datasheet template** introduced in *Datasheets for Machine Learning Sensors*. An ML sensor is an embedded edge device that encapsulates sensing, on-device ML processing, and data governance at the hardware boundary, while exposing a thin, sensor-like interface to the rest of the system. Learn more at: [mlsensors.org](https://mlsensors.org/).

![ML_sensor](https://github.com/harvard-edge/ML-Sensors/blob/main/figs/mlsensor.png)

## Repository metadata (FAIR and reuse)
This repository is designed to support **Findable, Accessible, Interoperable, and Reusable (FAIR)** usage of the datasheet template and example instantiations.

- **License:** See `LICENSE`
- **How to cite:** See `CITATION.cff` (or `CITATION`)
- **Authorship and contact:** See `AUTHORS.md` and the contact email below
- **Versioning and change history:** See `CHANGELOG.md` and the version history section in the template

**Contact:** <add-email-here>

## Quick start (use the template)
1. Open the editable template: [`template/ml_sensor_datasheet_template.md`](./template/ml_sensor_datasheet_template.md)
2. Duplicate it and fill it in for your ML sensor.
3. Export to PDF if desired (optional): `pandoc` or your preferred Markdown-to-PDF tool.
4. Submit improvements via pull request. Please include a brief note describing the change and update the version history.

## The ML sensor datasheet
The ML sensor datasheet provides a structured overview of the **hardware, data, model, privacy/security, and system-level behavior** relevant to an ML sensor. It builds on and unifies prior documentation approaches that describe parts of the pipeline, including:
- [Datasheets for datasets](https://arxiv.org/abs/1803.09010)
- [Data nutrition labels](https://arxiv.org/abs/1805.03677)
- [Model cards](https://arxiv.org/abs/1810.03993)
- Traditional hardware sensor datasheets

![related](https://github.com/harvard-edge/ML-Sensors/blob/main/figs/related.png)

The template covers topics including (not limited to): environmental impact, communication protocols, device diagrams, dataset attributes, model characteristics, end-to-end performance analysis, compliance and certifications, maintenance/versioning, and hardware specifications. The goal is to improve transparency, explainability, and auditability of ML sensors in real deployment contexts.

## Template and example datasheets (reproducibility)
To support reproducibility and adoption, this repository includes:
- An **editable, empty template** (Markdown):  
  [`template/ml_sensor_datasheet_template.md`](./template/ml_sensor_datasheet_template.md)
- Two **completed example datasheets** using the full template:
  - Open-source ML sensor datasheet (PDF):  
    [`open_source_datasheet_updated.pdf`](./open_source_datasheet_updated.pdf)
  - Commercial ML sensor datasheet (PDF):  
    [`commercial_datasheet_updated.pdf`](./commercial_datasheet_updated.pdf)

![datasheet](https://github.com/harvard-edge/ML-Sensors/blob/main/figs/datasheet_template.png)

## Versioning and updates
ML sensors may evolve over time due to firmware updates, model retraining, calibration changes, or hardware revisions. We therefore treat datasheets as **versioned artifacts**:
- Each release should specify the hardware/firmware/model version it documents.
- Updates should increment the datasheet version and summarize changes.
- When end-to-end performance changes, updated measurements should be reported and tied to the updated version.

## Contributing
Contributions are welcome. Please open an issue or submit a pull request.
- If you modify the template, update the template version history.
- If you add a new datasheet instance, include the filled template and (optionally) a PDF export.
- If you add figures or photos, include caption provenance (for example, “Photo by authors” or a source link).

