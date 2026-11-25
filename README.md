# Early Prediction of Mortality in Acute Kidney Injury Requiring Dialysis

Code repository for the study "Early Prediction of Mortality in Acute Kidney Injury Requiring Dialysis: A Comparative Analysis of Tabular Foundation Models and Conventional Machine Learning".

## Repository Content
* `early_prediction_of_mortality.ipynb`: End-to-end Google Colab / Python pipeline covering cohort curation at Time Zero, preprocessing regimes (`Raw`, `Minimal`, and `Preprocessed`), hyperparameter optimization (Optuna), model calibration, evaluation of conventional ML (`Logistic Regression`, `Random Forest`, `XGBoost`, `LightGBM`, `CatBoost`), tabular foundation models (`TabPFN 3.5`, `TabFM 1.0`), `FT-Transformer`, and `ModernBERT`, as well as fairness audits (`Fairlearn`), Decision Curve Analysis (DCA), and SHAP explainability.

## Environment & Required API Keys
All model training and inference run locally on GPU without transmitting clinical records to external APIs. To download pretrained weights for `TabPFN 3.5`, `TabFM 1.0` (`google/tabfm-1.0.0-pytorch`), and `ModernBERT` (`answerdotai/ModernBERT-base`), configure the following authentication tokens via environment variables or Colab Secrets:
* `TABPFN_TOKEN` / `TABPFN_API_KEY`
* `HF_TOKEN`

## Data Availability
In compliance with institutional ethics approval and the Brazilian General Data Protection Law (LGPD), individual-level patient data are not publicly deposited in this repository. De-identified analytical matrices may be requested from the corresponding author upon institutional approval.

## Citation
*Manuscript under review. Citation details (DOI and bibliographic reference) will be added upon publication.*

```bibtex
@article{franco2026early,
  title   = {Early Prediction of Mortality in Acute Kidney Injury Requiring Dialysis: A Comparative Analysis of Tabular Foundation Models and Conventional Machine Learning},
  author  = {Franco, Felipe de Oliveira and Smolentzov, Igor and Benedetto Filho, Marcos Sidney and Andrade, Lucia and Chiavegatto Filho, Alexandre Dias Porto},
  journal = {Journal of Medical Systems},
  year    = {2026},
  note    = {Under review; DOI to be added upon publication}
}
