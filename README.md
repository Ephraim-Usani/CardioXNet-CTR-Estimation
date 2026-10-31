# CardioXNet — Automated Cardiothoracic Ratio Estimation from Chest X-rays

> **CPU-optimized deep learning for cardiac screening in resource-constrained African hospitals**

[![Demo](https://img.shields.io/badge/▶%20Watch%20Demo-Google%20Drive-blue)](https://drive.google.com/file/d/1EBJdmsjtfyDvHqxXjMrhcvQx5_1X4Hj7/view)
[![Published](https://img.shields.io/badge/Published-Preprints%202025-green)](https://doi.org/10.20944/preprints202508.1478.v1)
[![CPU Only](https://img.shields.io/badge/Deployment-CPU%20Only-orange)]()
[![Python](https://img.shields.io/badge/Python-3.8+-yellow)]()

---

## The Clinical Problem

The Cardiothoracic Ratio (CTR) is one of the most important measurements in chest X-ray reporting. A CTR above 0.5 indicates cardiac enlargement — a critical finding in heart failure, cardiomegaly, and pericardial effusion.

Traditionally, radiologists measure CTR manually by drawing lines on the X-ray image. In high-volume hospitals across Sub-Saharan Africa, this manual process:
- Creates reporting delays in departments handling 100+ X-rays per day
- Introduces human measurement error and inter-observer variability
- Requires a trained radiologist — a scarce resource in rural Africa

**CardioXNet eliminates this bottleneck entirely.**

---

## What It Does

CardioXNet automatically:
1. Detects the cardiac silhouette and thoracic cavity on a chest X-ray
2. Measures the maximum cardiac diameter and maximum thoracic diameter
3. Calculates the CTR instantly and flags values above 0.5 as abnormal
4. Integrates results directly into a DICOM viewer for seamless clinical use

**Result: CTR estimation in under 3 seconds. No GPU required. No radiologist needed for measurement.**

---

## Why CPU-Only Matters

Most medical AI tools require expensive GPU hardware — completely impractical for district hospitals, mobile screening vans, and diagnostic centers across Nigeria and Sub-Saharan Africa.

CardioXNet was built from the ground up to run on **ordinary laptops and desktop computers** — the hardware that actually exists in African hospitals.

---

## Technical Approach

- **Model:** YOLOv8 Nano — chosen specifically for its CPU performance and small footprint
- **Dataset:** 3,000+ chest X-rays manually annotated under radiologist supervision
- **Architecture:** Custom segmentation pipeline for cardiac and thoracic boundary detection
- **Integration:** DICOM viewer plugin for direct clinical workflow integration
- **Performance:** Fast and reliable CTR estimation on CPU-only hardware

---

## Publication

> **Usani, E. U., Archibong, B. E., Egom, A. E., Efanga, S. A., Akintomide, A. O., Ukpong, E. V., Paulinus, S. O., Odukwu, F. I., & Egbe, N. O. (2025).** Automated cardiothoracic ratio estimation using CPU-based deep learning on chest X-rays: A novel approach in Sub-Saharan Africa. *Preprints*, 202508.1478.v1.
> [https://doi.org/10.20944/preprints202508.1478.v1](https://doi.org/10.20944/preprints202508.1478.v1)

---

## Demo

[▶ Watch CardioXNet in action](https://drive.google.com/file/d/1FeJMfrf0MtAP7UOIyve92g7k_fuKUbU2/view?usp=sharing)

---

## Built By

**Ephraim Usani** — First-Class Radiographer & Clinical AI Engineer, Lagos, Nigeria

[LinkedIn](https://www.linkedin.com/in/ephraim-usani) | [GitHub](https://github.com/Ephraim-Usani)

> *Built by someone who has measured CTRs manually in a Nigerian hospital — and decided to automate it.*
