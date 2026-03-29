# NAPT: Neural Array for Perceptual Text

> An assistive vision system that converts scene text into neural stimulation patterns for visually impaired users.

---

## Overview

NAPT is a research project exploring an end-to-end pipeline that:
1. Detects and recognizes text from real-world scenes (including degraded, low-visibility environments)
2. Translates recognized characters into electrode activation patterns via a custom **glyph-to-electrode mapping**
3. Delivers spatially encoded stimulation signals intended for cortical or retinal prosthetic devices

The core novelty is the glyph mapping layer — encoding character geometry directly into electrode activation arrays, designed to reduce required electrode density while preserving perceptual accuracy.

---

## Motivation

Millions of visually impaired individuals rely on assistive technologies that are either limited in scope or inaccessible. Existing visual prosthetics struggle with conveying text naturally. NAPT aims to bridge this gap by creating a principled, geometry-aware mapping from text characters to neural stimulation patterns — a translation layer with no direct prior implementation to reference.

---

## Planned Architecture

```
Input Image
    │
    ▼
Text Detection (EAST)
    │
    ▼
Text Recognition (TrOCR)
    │
    ▼
Glyph-to-Electrode Mapping
    │
    ▼
Electrode Activation Array
    │
    ▼
Neural Stimulation Output
```

---

## Project Status

| Phase | Status |
|---|---|
| Literature Review | ✅ Complete |
| System Architecture Design | 🔄 In Progress |
| OCR Pipeline (EAST + TrOCR) | ⏳ Planned |
| Glyph-to-Electrode Mapping | ⏳ Planned |
| Simulation & Validation | ⏳ Planned |

---

## Tech Stack *(planned)*

- **Python**
- **EAST** — Scene text detection
- **TrOCR** — Text recognition in degraded environments
- **PyTorch** — Model training and inference
- **NumPy / SciPy** — Electrode array encoding

---

## Repository Structure *(to be populated)*

```
napt/
├── docs/               # Literature review, design notes
├── src/
│   ├── detection/      # EAST-based text detection
│   ├── recognition/    # TrOCR pipeline
│   └── mapping/        # Glyph-to-electrode encoding
├── experiments/        # Simulation and validation scripts
├── assets/             # Diagrams, sample outputs
└── README.md
```

---

## Author

**Tarun Malepati**
MS Data Science, Indiana University
[LinkedIn](https://linkedin.com/in/tarun-malepati) · [GitHub](https://github.com/TarunMalepati99)

---

## License

This project is open for academic and research use. License to be added.
