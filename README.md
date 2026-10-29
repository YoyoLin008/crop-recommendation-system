# Crop Recommendation System

A Spring 2025 UIUC Data Science Club project exploring how soil nutrients and climate relate to crop choice. Built during my freshman year, the project combines exploratory visualizations, crop clustering, and a comparison of six classification models.

The notebooks use nitrogen, phosphorus, potassium, temperature, humidity, pH, and rainfall to classify 22 crop labels. This is an educational analysis of a small benchmark dataset; it has not been validated for farm planning or U.S. regional recommendations.

## Explore the project

| Notebook | What it covers |
| --- | --- |
| [01 · Crop exploration](notebooks/01_crop_exploration.ipynb) | Nutrient and climate distributions, correlations, and crop comparisons |
| [02 · Crop clustering](notebooks/02_crop_clustering.ipynb) | K-Means, hierarchical clustering, and PCA views of growing conditions |
| [03 · Model comparison](notebooks/03_model_comparison.ipynb) | Random Forest, XGBoost, LightGBM, SVM, KNN, and MLP classification |

Start with exploration, then clustering and model comparison. Each notebook can also run independently.

## Run locally

Use Python 3.12 and a fresh environment:

```bash
git clone https://github.com/YoyoLin008/crop-recommendation-system.git
cd crop-recommendation-system
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m jupyterlab
```

On Windows, activate the environment with `.venv\Scripts\activate` instead. Open a notebook in `notebooks/` and run its cells from top to bottom. Data paths work from the repository root or the notebook folder; no Colab upload is needed. If a new environment does not appear in Jupyter, restart Jupyter from the activated environment.

## Original model comparison

The original saved comparison used an 80/20 split with `random_state=42` and a scaler fitted only on the training data for SVM, KNN, and MLP.

| Model | Test accuracy |
| --- | ---: |
| Random Forest | 99.32% |
| XGBoost | 98.64% |
| LightGBM | 98.64% |
| MLP | 97.50% |
| SVM | 96.82% |
| KNN | 95.68% |

These are historical results from one split of 2,200 rows, not cross-validation or evidence of performance on new locations. Results may change with library versions. The clustering notebook is exploratory and does not measure crop suitability or profitability.

## Repository layout

```text
data/
  raw/                  Benchmark CSV and the original exploration ZIP
  processed/            Derived cluster tables and synthetic U.S. sample
notebooks/              Three numbered analysis notebooks
models/                 Legacy XGBoost model and usage notes
docs/                   Project history and cleanup notes
archive/placeholders/   Original incomplete file stubs, retained for reference
```

See the [data guide](data/README.md) for file descriptions and source limitations, the [model notes](models/README.md) for the legacy artifact, and the [project history](docs/project_history.md) for changes made during cleanup.

## Contributors

- **Yunya Lin** — [GitHub](https://github.com/YoyoLin008) · [LinkedIn](https://www.linkedin.com/in/yoyo-lin-631889299/)
- **Tianqi Zhang**
- **Sujia Guo** — [LinkedIn](https://www.linkedin.com/in/sujia-guo)

Developed collaboratively through the UIUC Data Science Club in Spring 2025.

## License

Project code and original documentation are available under the [MIT License](LICENSE). Third-party datasets, their derivatives, and pretrained model artifacts are covered separately; see [NOTICE.md](NOTICE.md) and the [data guide](data/README.md). The code license does not establish rights to redistribute source data.
