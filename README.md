# Lightweight Machine Learning for Detecting DGA-Based Botnet Communications

## Paper

*“Lightweight Machine Learning for Detecting DGA-Based (Domain Generation Algorithm Based) Botnet Communications,”* submitted to ECE239AS (June 2026).  

**PDF:** ./paper_final.pdf

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter lab
```

Run the notebooks in `notebooks/artifacts/` to regenerate the paper figures.

## Directory Guide
| Path | Purpose |
|------|---------|
| `data/backup_csvs/` | Open datasets committed to the repo in case the online copy is updated. |
| `data/raw/` | Placeholder for local or derived data files. |
| `data/sql/` | SQL files, if future data sources require them. |
| `notebooks/artifacts` | Jupyter workflows (analysis + plots). |
| `notebooks/models` | Jupyter workflows (data + superfluous plots). |
| `scripts/` | Notes on the script-free notebook workflow. |
| `figures/` | Auto-generated paper artifacts. |

## Artifact Map

| Paper artifact | Notebook | Output |
|------|------|------|
| Figure 1 | `notebooks/artifacts/fig1_distribution_of_vowel_and_digit_ratios.ipynb` | `figures/ratio.pdf` |
| Figure 2 | `notebooks/artifacts/fig2_correlation_heatmap_of_lexical_features_and_class_label.ipynb` | `figures/features.pdf` |
| Figure 3 | `notebooks/artifacts/fig3_dga_domain_families.ipynb` | `figures/families.pdf` |
| Figure 4 | `notebooks/artifacts/fig4_domain_length_distribution_by_dga_family.ipynb` | `figures/kde.pdf` |
| Figure 5 | `notebooks/artifacts/fig5_random_forest_feature_importance.ipynb` | `figures/RandomForestFeatureImportanceF1-ScoreMetric-50-50.pdf` |
| Figure 6 | `notebooks/artifacts/fig6_singular_decision_tree_from_random_forest.ipynb` | `figures/decision_tree.pdf` |
| Figure 7 | `notebooks/artifacts/fig7_roc_auc.ipynb` | `figures/roc_auc.pdf` |
