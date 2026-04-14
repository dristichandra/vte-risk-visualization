# Visualizing Cancer-Associated Blood Clot Risk Over Time

An evidence-based visualization framework for communicating venous thromboembolism (VTE) risk to clinicians and cancer patients.

## Overview

Current VTE risk assessment tools achieve 95%+ prediction accuracy (AUROC) but face 49–96% clinical alert override rates. The gap is not prediction — it is communication. This project presents the first empirically-grounded temporal visualization framework for VTE risk in cancer patients, synthesizing principles from medical informatics, human-computer interaction, and implementation science.

## Research Team

- **Dristi Chandra** — Undergraduate Researcher, University of Washington
- **Kavya Chandrasekar** — Co-Researcher, University of Washington
- **Dr. Barbara Lam** — Faculty Advisor, Fred Hutchinson Cancer Center

## Design Principles

The framework is built on four evidence-based design principles:

1. **Counting over Calculating** — Quantile dots over error bars (1.4x better comprehension; Padilla 2023)
2. **Temporal Narrative over Static** — Dynamic risk trajectories over point-in-time snapshots (28% improvement in early detection; Kia 2021)
3. **Transparency over Black-Box** — Explainable risk factors over unexplained algorithms (67% override rate for opaque models)
4. **Passive Integration over Alerts** — Workflow-embedded displays over interruptive pop-ups (12% workflow error increase from alerts)

## Project Structure

```
vte-risk-visualization/
├── README.md
├── LICENSE
├── .gitignore
├── docs/                   # Research documentation
│   ├── poster/             # Symposium poster files
│   └── paper/              # Manuscript drafts
├── literature/             # Systematic review materials
│   ├── search-strategy.md  # Database queries and inclusion criteria
│   └── references.bib      # BibTeX references
├── design/                 # Design artifacts
│   ├── wireframes/         # Visualization wireframes
│   └── principles/         # Design principle documentation
├── prototype/              # Interactive prototype (React + D3.js)
│   ├── src/
│   └── package.json
└── figures/                # Charts and figures for poster/paper
```

## Methods

1. **Systematic Literature Review** — PRISMA protocol examining studies across dynamic risk prediction, uncertainty visualization, and clinical decision support implementation
2. **Clinical Workflow Analysis** — Shadowing oncologists at Fred Hutch to understand decision context, information needs, and existing tool integration
3. **Iterative Design Process** — Wireframe prototypes developed with hematologist consultation, incorporating evidence-based principles from HCI research
4. **Interactive Prototype Development** — Functional React-based visualization using D3.js for charts and FHIR integration for EHR compatibility

## Visualization Framework Components

- **Patient View** — Temporal risk trajectory with quantile dot uncertainty display
- **PRISM View** — Multi-factor transparency panel showing contributing risk factors
- **Clinical Integration** — Passive EHR-embedded display designed for existing workflows

## Status

- [x] Systematic literature review (n=50 studies)
- [x] Clinical workflow shadowing at Fred Hutch
- [x] Evidence-based design principles established
- [x] Wireframe prototypes developed
- [ ] Interactive prototype (in progress)
- [ ] IRB application — clinician usability study (in progress)
- [ ] Usability evaluation (planned)

## Presentations

- **ITHS Symposium** — UW Seattle, May 12, 2026 (poster presentation)

## Built With

- React
- D3.js
- FHIR (HL7)

## License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.

## Acknowledgments

This research is conducted at the Fred Hutchinson Cancer Center and the University of Washington. We thank the oncology clinicians at Fred Hutch/UW Medicine who participated in workflow shadowing and design consultation.
