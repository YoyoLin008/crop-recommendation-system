# Legacy model artifact

`xgboost_model.pkl` is the original Spring 2025 serialized XGBoost artifact. It is preserved for reference and is not required by the three analysis notebooks, which train their models in memory.

The artifact's complete training procedure, preprocessing objects, feature order, label mapping, library versions, and evaluation record are not bundled here. It is therefore not a supported prediction interface. Use the model comparison notebook to retrain an inspectable model rather than assuming this pickle matches its results.

Only load pickle files from a source you trust; loading a pickle can execute code. Upstream data and model rights are separate from the code's MIT License; see [NOTICE.md](../NOTICE.md).

The previous `env_soil_model.pkl` in GitHub was a two-byte stub, not a working model. Its original bytes are retained under [archive/placeholders](../archive/placeholders/).
