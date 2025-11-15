# Interpretable Credit Risk Modeling (SHAP & LIME)

This repository contains a GitHub-ready project for building interpretable machine learning models
to predict credit default and generate both global (SHAP) and local (LIME) explanations.

## Structure

```
credit_risk_project/
├── data/
│   └── credit_data.csv
├── notebooks/
│   └── credit_risk_interpretability.ipynb
├── src/
│   ├── train.py
│   └── interpret.py
├── artifacts/         # models, scaler, feature names (created after running training)
├── interpretations/   # SHAP images and LIME html files (created after running interpret)
├── requirements.txt
├── README.md
└── LICENSE
```

## Quickstart

1. Create a virtual environment:

    ```bash
    python -m venv venv
    source venv/bin/activate   # macOS / Linux
    venv\Scripts\activate    # Windows
    ```

2. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. Train models:

    ```bash
    python -m src.train
    ```

4. Generate SHAP & LIME explanations:

    ```bash
    python -m src.interpret
    ```

5. Open the notebook for walkthroughs:

    ```bash
    jupyter notebook notebooks/credit_risk_interpretability.ipynb
    ```

## Notes

- The `data/credit_data.csv` provided is a synthetic sample for demonstration. Replace it with your own dataset for real experiments.
- Artifacts (trained models and scaler) are saved into `artifacts/` after training.
- Interpretations are saved into `interpretations/`.