---
template: home.html
title: H → WW NanoAOD Analysis
---

## What This Analysis Does

This analysis searches for the **Standard Model Higgs boson** ($m_H = 125\,\text{GeV}$) decaying
to a pair of $W$ bosons in the opposite-flavour dilepton final state:

$$gg \rightarrow H \rightarrow W^+W^{-*} \rightarrow e^\pm\,\nu_e\;+\;\mu^\mp\,\nu_\mu$$

The analysis strategy follows the approach described in the CMS H→WW measurement
([Tumasyan et al., _Eur. Phys. J. C_ **83**, 667, 2023](https://doi.org/10.1140/epjc/s10052-023-11632-6)),
adapted for CMS Open Data using the Scikit-HEP Python ecosystem.

## Key Analysis Properties

| Quantity              | Value                                               |
| --------------------- | --------------------------------------------------- |
| Centre-of-mass energy | $\sqrt{s}=13~\mathrm{TeV}$                          |
| Data-taking period    | 2016 Ultra-Legacy (Run periods G–H)                 |
| Integrated luminosity | $\mathcal{L}_{\mathrm{int}}=16.39~\mathrm{fb}^{-1}$ |
| Signal process        | $ggH \rightarrow W^+W^- \rightarrow e\nu\mu\nu$     |

## Pre-Requisite

- This analysis assumes a basic working knowledge of `Python`, including familiarity with functions, dictionaries, lists, and arrays.
- Readers are also expected to have prior exposure to undergraduate or graduate-level particle physics, along with an understanding of standard terminology related to fundamental particles.

---

## Quick Start

```bash title="Get up and running"
# 1. Clone the repository
git clone https://github.com/anrghv/H-to-WW-NanoAOD-analysis.git
cd H-to-WW-NanoAOD-analysis

# 2. Create the environment (Conda recommended)
conda env create -f environment.yml
conda activate HEP_analysis

# 3. Open the main analysis notebook
cd notebooks/
jupyter lab HWW_analysis.ipynb
```

→ Full setup instructions: [Installation & Setup](getting-started/installation.md)

---

## Documentation Guide

| Section                                                    | Description                                            | Link                                                                      |
| ---------------------------------------------------------- | ------------------------------------------------------ | ------------------------------------------------------------------------- |
| :material-book-open-variant: **Physics Background**        | CMS Open Data, Higgs signal, and background processes. | [:octicons-arrow-right-24: Theory](theory/higgs-physics.md)               |
| :material-database: **Datasets**                           | Sample list, cross-sections, and MC normalisation.     | [:octicons-arrow-right-24: Datasets](datasets/data-and-mc.md)             |
| :material-wrench: **Software Framework**                   | The Scikit-HEP ecosystem explained.                    | [:octicons-arrow-right-24: Framework](software/ecosystem.md)              |
| :material-download: **Installation & Setup**               | Environment setup and verification.                    | [:octicons-arrow-right-24: Installation](getting-started/installation.md) |
| :material-chart-timeline-variant: **Analysis Methodology** | Analysis methodology and Jupyter notebook.             | [:octicons-arrow-right-24: Methodology](analysis/methodology.md)          |
| :material-chart-bar: **Statistical Inference**             | CMS Combine: datacards, signal strength.               | [:octicons-arrow-right-24: Combine](combine/statistical-inference.md)     |

---

<!-- ## Acknowledgements -->

<!-- This analysis is developed as part of the [**HSF-India project**](https://research-software-collaborations.org/). Datasets are sourced from the
[CERN Open Data Portal](https://opendata.cern.ch). MC sample configurations follow
[LatinoAnalysis](https://github.com/latinos/LatinoAnalysis) conventions for the Summer20UL16 campaign. -->

## Acknowledgements

- This analysis is developed as part of the [**HSF-India project**](https://research-software-collaborations.org/).
- Datasets are sourced from the [CERN Open Data Portal](https://opendata.cern.ch).
- MC sample configurations follow [LatinoAnalysis](https://github.com/latinos/LatinoAnalysis)
  conventions for the Summer20UL16 campaign. The ggH selection strategy is based on the
- CMS H→WW measurement: A. Tumasyan et al. (CMS Collaboration),
  [_Eur. Phys. J. C_ **83**, 667 (2023)](https://doi.org/10.1140/epjc/s10052-023-11632-6).
