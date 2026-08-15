# Data Directory

## Current Status and Policy

No dataset has been acquired for this project. Raw data must not be uploaded directly to the GitHub repository. After an authorized dataset is obtained separately, record its provenance, license, download date, version, and integrity information before analysis.

The intended scope is real PLGA nanoparticle formulation data for small-molecule drugs prepared by nanoprecipitation. Dataset contents and exact columns have not yet been verified.

## Planned Fields

The following are expected fields for planning purposes only. They are not claims about the columns available in any future dataset.

| Category | Planned information, subject to verification |
| --- | --- |
| Drug-related | Molecular structure, aqueous solubility, logP, molecular weight, polarity, and hydrogen-bond-related properties |
| PLGA and formulation | LA:GA ratio, PLGA molecular weight, and drug-to-polymer ratio |
| Manufacturing conditions | Solvent properties, surfactant or stabilizer conditions, aqueous-to-organic phase ratio, and pH |
| Main outcomes | Encapsulation efficiency and particle size |

For every verified column, the data documentation must record the source column name, normalized name if used, definition, reported unit, any unit conversion, data type, and missing-value convention. Units and definitions must come from the actual source rather than assumption.

## Dataset Provenance Record

- Dataset title:
- Data source:
- DOI or official URL:
- License:
- Download date:
- Data version or checksum:
- Notes:

Complete this record separately for each acquired source.

## Data Lifecycle

- `raw/`: An immutable copy of acquired source files. Never edit these files directly.
- `interim/`: Reproducible intermediate outputs created while cleaning, harmonizing, or validating raw data.
- `processed/`: Analysis-ready data produced from documented transformations.

These directories are excluded from Git. Transformation logic, schemas, and provenance records should remain version-controlled when they are implemented.

## Data Integrity

Do not create fictional experimental rows, literature records, or measurement values. If real data is unavailable, document only required structures, planned fields, definitions, and units. Synthetic fixtures may later be used only for unit-test format checks, never for model training, performance evaluation, or scientific reporting.
