```markdown
# Household Decision-Influence Analysis

**Author :** Aziz Ben Jemia  
**Scope :** 22 368 survey observations · Naivasha, Kenya  
**Goal :** Quantify which factors increase a woman’s influence over household decisions.

---

## 🔍 Project Snapshot
- **Problem type** : Binary classification (`influence` vs `no-influence`)
- **Features** : Schooling, insurance, earning power, parity, marital status
- **Models** : Baseline → Logistic Reg → Interaction Logit (best fit)
- **Key metric** : Macro-F1 (class-balanced accuracy)

---

## 📂 Repo Layout
```

household-decision-influence-analysis/
├── data/            # Raw Excel + cleaned CSV
├── notebooks/       # Main analysis (EDA → modelling)
├── src/             # Re-usable preprocessing & modelling code
├── reports/figures/ # Auto-saved charts
├── environment.yml  # Conda setup (Python 3.11)
└── README.md

````

---

## 🚀 Quick Start
```bash
git clone https://github.com/azizbenjemia/household-decision-influence-analysis.git
cd household-decision-influence-analysis
conda env create -f environment.yml
conda activate decision-influence
jupyter lab notebooks/analysis.ipynb
````

---

## 📊 Highlight Results

| Insight                                             | Evidence                                                        |
| --------------------------------------------------- | --------------------------------------------------------------- |
| **Education boosts influence**                      | +18 pp in predicted probability from primary → higher education |
| **Insurance × Education interaction** is *negative* | Diminishing marginal effect once both are present               |
| **Main earner = lower odds of influence**           | Suggests traditional gender roles still dominate                |

Best model (interaction logit) reaches **Pseudo-R² = 0.128** and **Macro-F1 = 0.71**.

---

## ⚙️ Reproduce via CLI

```bash
python -m src.modelling --config configs/base.yaml
# Figures will appear in reports/figures/
```

---

## ➡️ Next Steps

1. Add income quantiles instead of binary earner flag.
2. Test tree-based models (e.g., XGBoost) for non-linear effects.
3. Deploy a small Streamlit dashboard for interactive scenario testing.

---

## 📜 License

MIT – see `LICENSE`.

---

## 🙋 Contact

[GitHub @azizbenjemia](https://github.com/azizbenjemia) · [azizbenjemia@example.com](mailto:azizbenjemia@example.com)

```
```

