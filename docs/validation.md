# Validation record

Checked on October 29, 2026 with Python 3.12.14 on macOS.

All three notebooks executed from top to bottom: **50 code cells, zero errors**. Execution used copies outside the repository, leaving the labeled historical outputs intact. Data path discovery was checked from both the repository root and the notebook folder. Documentation links resolve, and the moved data, placeholders, and legacy model retain their original content hashes.

The rerun reproduced the original model comparison accuracy values in the README. This checks execution and consistency on the included benchmark; it does not add geographic or agronomic validation.

| Package | Version |
| --- | --- |
| numpy | 2.5.4 |
| pandas | 2.3.3 |
| scipy | 1.18.1 |
| scikit-learn | 1.9.1 |
| xgboost | 3.4.1 |
| lightgbm | 4.7.0 |
| matplotlib | 3.11.2 |
| seaborn | 0.13.2 |
| plotly | 6.9.0 |
| jupyterlab | 4.6.5 |
| ipykernel | 6.31.0 |
| nbclient | 0.11.0 |
| nbformat | 5.11.1 |

The ranges in `requirements.txt` allow compatible upgrades. This table records the versions used for this check, not a complete dependency lock.
