# PLM-indicators

**Population Learning Management (PLM) Dashboard Indicator Catalog**

This repository contains the complete catalog of 62 indicators that constitute the PLM dashboard design, a Design Science Research artifact that transfers Population Health Management (PHM) constructs to K-12 educational decision-making.

This repository accompanies the paper:

> Sasano, K. (2026). Population Learning Management: Transferring Population Health Management to K-12 Educational Dashboard Design. [Conference / Journal name, to be updated]

---

## Overview

PLM organizes 62 indicators across **six domains** and **three administrative layers** (Macro / Meso / Micro) to support population-scale educational decision-making while preserving professional judgment.

The indicator catalog is intended as a design-phase artifact. It specifies what each indicator measures, where the data comes from, how often it should be updated, and what threshold triggers attention. Empirical validation through phased deployment is planned in future work.

---

## Six Domains

| Code | Domain Name | PHM Counterpart |
|------|-------------|-----------------|
| **LVS** | Learning Vital Signs | Vital signs (temperature, blood pressure, pulse) |
| **LRS** | Learning Risk Stratification | Disease risk stratification (Kaiser Pyramid) |
| **SDoL** | Social Determinants of Learning | Social Determinants of Health (SDoH) |
| **IE** | Intervention Effectiveness | Treatment effects / clinical outcomes |
| **RE** | Resource Efficiency | Healthcare cost / resource optimization |
| **LE** | Learning Engagement | Patient engagement |

See `docs/` for detailed documentation of each domain.

---

## Indicator Distribution

| Domain | Macro | Meso | Micro | Total |
|--------|-------|------|-------|-------|
| LVS    |   5   |   5  |   3   |  13   |
| LRS    |   4   |   3  |   3   |  10   |
| SDoL   |   5   |   3  |   2   |  10   |
| IE     |   4   |   3  |   3   |  10   |
| RE     |   4   |   3  |   3   |  10   |
| LE     |   3   |   3  |   3   |   9   |
| **Total** | **25** | **20** | **17** | **62** |

---

## Repository Structure

    PLM-indicators/
    ├── README.md                    # This file
    ├── LICENSE                      # CC BY 4.0
    ├── CITATION.cff                 # Citation metadata
    ├── CHANGELOG.md                 # Version history
    ├── indicators/
    │   ├── indicators-master.csv    # Complete 62-indicator catalog
    │   ├── indicators-master.xlsx   # Excel version
    │   └── indicators-master.json   # JSON version
    └── docs/
        ├── domain-LVS.md            # Learning Vital Signs (13 indicators)
        ├── domain-LRS.md            # Learning Risk Stratification (10 indicators)
        ├── domain-SDoL.md           # Social Determinants of Learning (10 indicators)
        ├── domain-IE.md             # Intervention Effectiveness (10 indicators)
        ├── domain-RE.md             # Resource Efficiency (10 indicators)
        └── domain-LE.md             # Learning Engagement (9 indicators)

---

## Indicator ID Convention

Each indicator has a unique ID in the format **Layer-Domain-Number**:

- **Layer prefix**: `M` (Macro / educational authority), `S` (School / meso), `T` (Teacher / micro / classroom)
- **Domain code**: LVS / LRS / SDoL / IE / RE / LE
- **Number**: Two-digit sequence within layer-domain combination

Examples:
- `M-LVS-01`: First Macro-layer indicator in Learning Vital Signs
- `T-IE-03`: Third Micro-layer indicator in Intervention Effectiveness
- `S-SDoL-02`: Second Meso-layer indicator in Social Determinants of Learning

---

## CSV Schema

Each row in `indicators-master.csv` contains the following fields:

| Field | Description |
|-------|-------------|
| `ID` | Unique identifier (Layer-Domain-Number) |
| `Domain` | One of LVS / LRS / SDoL / IE / RE / LE |
| `Layer` | One of Macro / Meso / Micro |
| `Indicator_Name_EN` | English name |
| `Indicator_Name_JP` | Japanese name |
| `Definition` | One- to two-sentence definition |
| `Data_Source` | Source data system or instrument |
| `Update_Frequency` | daily / weekly / monthly / quarterly / annually |
| `Threshold` | Alert threshold (numerical or qualitative) |
| `Decision_Owner` | Role responsible for acting on this indicator |
| `Action_Trigger` | Recommended action when threshold is exceeded |
| `Rationale` | Why this indicator was selected (PHM correspondence) |

---

## How to Cite

If you use the PLM indicator catalog in your research or practice, please cite the accompanying paper:

    @inproceedings{sasano2026plm,
      author    = {Sasano, Kento},
      title     = {Population Learning Management: Transferring Population Health Management to K-12 Educational Dashboard Design},
      booktitle = {[Conference Proceedings, to be updated]},
      year      = {2026}
    }

When referring directly to the indicator catalog, please also include the repository URL:

> Sasano, K. (2026). *PLM Indicator Catalog: 62-Indicator Design Specification for Population Learning Management*, Version 1.0.0. Available at: https://github.com/PLM-research/PLM-indicators

---

## License

This work is licensed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**.

You are free to share and adapt the material for any purpose, including commercial use, provided that you give appropriate credit.

See [LICENSE](LICENSE) for the full license text.

---

## Status

- **Version**: 1.0.0
- **Status**: Design-phase artifact (not yet empirically validated)
- **Next steps**: Phased pilot deployment via Design-Based Implementation Research (DBIR) partnership with a Japanese prefectural board of education

---

## Contact

Kento Sasano
Faculty of Environmental, Life, Natural Science and Technology, Okayama University
ORCID: 0009-0009-3853-8029

---

## Repository URL

https://github.com/PLM-research/PLM-indicators
