# Project history

## Spring 2025

Freshman-year UIUC Data Science Club project by Yunya Lin, Tianqi Zhang, and Sujia Guo. The public repository preserves crop exploration, environmental clustering, and a six-model benchmark comparison.

## Repository cleanup — October 2026

- Numbered the three notebooks and made their data paths work from either the repository root or `notebooks/`.
- Removed the identical root-level notebook copy; organized inputs under `data/raw/` and derived tables under `data/processed/`.
- Kept the two historical benchmark copies and the original legacy model. Archived unusable placeholder files without replacing them with unrelated local assets.
- Replaced the Colab upload step with a local ZIP path.
- Corrected the comparison notebook's final XGBoost plot, which previously displayed LightGBM predictions.
- Removed `env_cluster` from the inputs used to predict `env_cluster`. Removed numeric cluster identifiers from crop-average environmental features. Old affected clustering outputs were cleared before verification.
- Corrected the README's original claim that XGBoost had the highest accuracy; the saved comparison ranks Random Forest first.
- Added setup instructions, a focused dependency list, MIT licensing for code and original documentation, and separate data/model attribution notes.

These changes improve readability and execution without turning the project into a validated agricultural recommendation service. Cluster assignments and model outputs can change after the corrections or with different library versions.

## Local-only work

The original DataDive folder also contains soil/climate merges, incomplete notebooks, figures, trained artifacts, and a later U.S. county recommender. That later experiment uses seeded county profiles and synthetic historical data and is separate from the Spring 2025 benchmark. These local materials are not added to the public repository as part of this cleanup.
