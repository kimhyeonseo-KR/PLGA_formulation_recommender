# PLGA Formulation Recommender

## Overview

PLGA Formulation Recommender is a planned Python decision-support project for experimental prioritization of PLGA nanoparticle formulations prepared by nanoprecipitation. Its long-term purpose is to help screen formulation candidates for a new small-molecule drug that was not included in the training data. The system is intended to combine molecular properties with evidence from existing PLGA formulation records and rank candidates that may be worth testing first.

The first planned version will focus on two model-estimated outcomes:

- encapsulation efficiency
- particle size

## Current Status

Only the initial project structure and documentation exist. No dataset has been acquired, and no data loading, preprocessing, machine learning, prediction, candidate generation, ranking, API, CLI, or user interface has been implemented. There is currently no executable workflow.

## Intended Use and Limitations

Future outputs are intended for candidate recommendation and candidate screening under limited experimental resources. They must support, not replace, scientific judgment. Any recommended conditions and model-estimated outcomes will require experimental confirmation. The project is not an experimentally validated formulation system, and its applicability to a new drug will depend on how well that drug and the proposed conditions are represented by the evidence used for development.

## Planned Inputs

Expected input information, subject to confirmation against real datasets, includes:

- Drug properties: molecular structure, aqueous solubility, logP, molecular weight, polarity, and hydrogen-bond-related properties.
- PLGA and formulation properties: LA:GA ratio, PLGA molecular weight, drug-to-polymer ratio, solvent properties, surfactant or stabilizer conditions, aqueous-to-organic phase ratio, and pH.

Actual field names, definitions, units, and availability will be documented only after real data is inspected.

## Planned Outputs

The planned output is a ranked set of PLGA formulation and manufacturing-condition candidates for experimental prioritization. Each candidate may eventually include model-estimated encapsulation efficiency and particle size, together with applicability and uncertainty information. No such output is generated at the current stage.

## Development Path

Development will proceed from data acquisition and schema verification to baseline outcome models, molecular-property integration, candidate generation, ranking, uncertainty communication, and a user interface. See [docs/roadmap.md](docs/roadmap.md) for completion criteria and current status.

## Repository Structure

```text
.
├── README.md
├── AGENTS.md
├── .gitignore
├── requirements.txt
├── data/
│   └── README.md
├── docs/
│   ├── roadmap.md
│   └── experiment_log.md
├── notebooks/
│   └── .gitkeep
├── src/
│   └── plga_recommender/
│       └── __init__.py
└── tests/
    └── .gitkeep
```

## Data Policy

Downloaded source data, intermediate datasets, large processed datasets, trained models, and model artifacts are not stored directly in this repository. Data must be obtained separately from authorized sources. Its provenance, license, download date, version or checksum, column definitions, and units must be recorded before use; see [data/README.md](data/README.md).
