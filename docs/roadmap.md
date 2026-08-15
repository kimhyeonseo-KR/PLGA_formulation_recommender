# Development Roadmap

Only Stage 1 is complete. All later stages are planned and have not started.

| Stage | Purpose | Completion criteria | Status |
| --- | --- | --- | --- |
| 1. Create the project structure | Establish the minimal repository layout, scope, and contribution rules. | All requested scaffold files and directories exist and accurately document the current state. | Complete |
| 2. Acquire a real PLGA formulation dataset | Obtain authorized evidence for small-molecule PLGA nanoparticles prepared by nanoprecipitation. | Source files are obtained outside Git and provenance and license records are completed. | Planned - not started |
| 3. Inspect data files and column names | Determine what the acquired files actually contain. | File inventory, source column list, and initial schema are documented from real files. | Planned - not started |
| 4. Verify sources, units, and missing values | Make the data interpretable and auditable before modeling. | Definitions, units, missing-value conventions, versions, and checksums are recorded. | Planned - not started |
| 5. Implement a baseline encapsulation-efficiency model | Establish a reproducible first outcome estimate. | A documented baseline is trained and evaluated on verified real data. | Planned - not started |
| 6. Add particle-size prediction | Extend outcome estimation to particle size. | A reproducible particle-size baseline and evaluation are documented. | Planned - not started |
| 7. Calculate SMILES-based drug properties | Represent drug structure with reproducible molecular features. | Descriptor definitions, calculation code, validation, and failure handling are documented. | Planned - not started |
| 8. Connect an existing aqueous-solubility model | Add a relevant drug property without silently treating estimates as measurements. | Model provenance, interface, validation, units, and limitations are documented. | Planned - not started |
| 9. Generate formulation candidates for a new drug | Create constraint-aware PLGA and nanoprecipitation condition candidates. | Candidate rules and valid ranges are documented and tested. | Planned - not started |
| 10. Estimate outcomes for each candidate | Attach model-estimated encapsulation efficiency and particle size. | Each candidate receives reproducible estimates with model/version metadata. | Planned - not started |
| 11. Rank candidates by user goals | Support experimental prioritization under explicit preferences. | Ranking objectives, trade-offs, tie handling, and tests are documented. | Planned - not started |
| 12. Show applicability and uncertainty | Communicate limits when a new drug differs from development data. | Domain checks, uncertainty outputs, and user-facing warnings are implemented and validated. | Planned - not started |
| 13. Implement a user interface | Make inputs, candidate results, and limitations accessible. | A documented interface supports the validated workflow and displays uncertainty. | Planned - not started |
| 14. Review iterative recommendation from experimental results | Assess a future feedback loop using newly observed laboratory results. | A design and governance review defines whether and how updates should occur. | Planned - not started |
