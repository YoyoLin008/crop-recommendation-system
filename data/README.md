# Data guide

| File | Contents | Use |
| --- | --- | --- |
| `raw/Crop_recommendation.csv` | 2,200 rows, seven numeric inputs, 22 crop labels | Model comparison |
| `raw/crop_exploration.zip` | Original `Data Set.zip`; contains a 2,200-row `Crop_recommendation.csv` with expanded nutrient names and two empty columns | Crop exploration |
| `processed/Crop_recommendation_with_clusters.csv` | 2,200 rows with `env_cluster` and expanded nutrient names | Crop clustering |
| `processed/final_crop_clusters.csv` | Historical 22-crop summary with environmental means and cluster columns | Reference output; not regenerated automatically |
| `processed/Crop_recommendation_US.csv` | 600 synthetic samples for six crops | Early experiment; not measured U.S. field data |

The benchmark CSV uses `N`, `P`, `K`, `temperature`, `humidity`, `ph`, `rainfall`, and `label`. The exploration and clustering copies use `Nitrogen`, `phosphorus`, and `potassium` instead of `N`, `P`, and `K`. The exploration notebook removes the ZIP's empty columns before plotting correlations.

The raw CSV and the CSV inside the ZIP are different historical copies, so both are retained. Renaming a file to include `US` does not establish geographic coverage. The local generator for the U.S. sample draws random values from manually specified crop ranges; this dataset must not be used as evidence of regional accuracy.

The local project cites [this Kaggle distribution](https://www.kaggle.com/datasets/aksahaha/crop-recommendation). Exact upstream versions, units for all nutrient fields, sampling geography, and redistribution terms were not documented. See [NOTICE.md](../NOTICE.md). The repository contains no verified U.S. location or farm-level evaluation dataset.

The small files previously named `Crop recommendation dataset.csv` and `最终整合推荐结果Top3.xlsx` were descriptive or empty stubs. They are retained under [archive/placeholders](../archive/placeholders/) rather than listed as usable datasets. Larger local soil and climate files are kept in the local workspace archive.
