# Repository Guidelines

## Project Structure & Module Organization

Keep the root limited to project-level files such as `README.md`, dependency manifests, and tool configuration. Place implementation under `src/`, automated tests under `tests/`, documentation under `docs/`, notebooks under `notebooks/`, and data documentation under `data/`. Use `plga_recommender` as the Python package name and keep its importable code under `src/plga_recommender/`; mirror future source modules in `tests/`.

Do not commit large formulation datasets, generated models, or experiment outputs. Document how to obtain them, including versions and checksums, in `docs/`.

## Build, Test, and Development Commands

No build, test, lint, formatting, CLI, or run command is configured yet. `requirements.txt` is currently a placeholder. Do not present `pytest`, `ruff`, a package entry point, or any other tool as available until its configuration and runnable code are committed. When a toolchain is added, document reproducible commands in `README.md`. Do not rely on globally installed, undocumented tools.

## Coding Style & Naming Conventions

Use four-space indentation for Python. Once a formatter is configured, let it control layout. Prefer simple, readable Python and small, typed functions. Name modules, functions, and variables with `snake_case`, classes with `PascalCase`, and constants with `UPPER_SNAKE_CASE`. Use meaningful names that expose scientific units, such as `particle_size_nm` or `drug_loading_percent`. Avoid ambiguous abbreviations and unexplained formulation assumptions.

Implement one clearly scoped feature per task. Do not add unrequested features or expand the requested scope. Update related README sections and documentation whenever behavior is added or changed.

## Testing Guidelines

No test framework is configured yet. When tests are introduced, mirror source modules with files named `tests/test_<module>.py` and name tests by behavior, for example `test_rejects_negative_polymer_ratio`. Synthetic data is permitted only in unit-test fixtures that verify data formats and structures. Never use synthetic data for model training, performance evaluation, or scientific reporting.

## Data Integrity & Scientific Boundaries

Never invent experimental measurements, formulation rows, or literature data. If real data is unavailable, document only the planned fields, definitions, units, and data structure. For every acquired dataset, record its source, license, version or checksum, column definitions, and units.

Keep `data/raw/`, `data/interim/`, and `data/processed/` conceptually separate. Treat raw data as immutable; transformations must create new interim or processed outputs. Model outputs are decision-support estimates, not confirmed formulation conditions. Evaluate applicability to unseen drugs and communicate domain limitations and uncertainty.

## Commit & Pull Request Guidelines

There is no existing Git history to derive a convention from. Use short, imperative commits with a clear prefix, such as `feat: add release-profile scoring` or `test: cover missing molecular weight`. Keep each commit focused.

Do not run `git add`, `git commit`, or `git push`, create a GitHub repository, delete files, install packages, or download data without the user's explicit permission.

Pull requests should explain the problem and approach, list validation commands and results, identify data or model assumptions, and link relevant issues. Include screenshots for user-interface changes and note any compatibility or configuration impact. After changing code or documentation, report every created or modified file and every command executed.

## Security & Configuration

Never store API keys, credentials, personal or patient information, proprietary datasets, non-public data, or local `.env` files in the repository. Review new dependencies and data licenses before merging.
