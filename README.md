# Household Decision-Making Influence – Logistic Regression Study


A  data-science project that explores **which factors empower women to influence household decisions** in rural Naivasha, Kenya.  
Using a survey-based discrete-choice experiment (DCE) of **22 368 observations** we fit and interpret several logistic-regression models to answer:

> *How do education, insurance coverage, earnings power and reproductive history shape a woman's influence in household decision-making?*

---

## 1. Project motivation

Women’s autonomy is a recognised determinant of maternal and child health outcomes. However, quantitative evidence on *drivers* of intra-household influence is still limited.  
This study leverages a rich DCE dataset to quantify the effect sizes of:

| Variable | Proxy for | Rationale |
|----------|-----------|-----------|
| `schooling` | Educational attainment | Education often increases bargaining power |
| `motherhoodinsurance` | Financial security | Insurance may signal economic independence |
| `mainearner` | Relative income | Direct measure of household bargaining position |
| `motherhoodpregnancyexperiencetim` | Parity | Larger families may redistribute influence |
| `married` | Marital status | Marriage can formalise joint decision structures |

The binary outcome **`hohnoinfluence`** equals **1** if the respondent reports influence over household decisions and **0** otherwise :contentReference[oaicite:8]{index=8}.

---

## 2. Data

| Source | Citation |
|--------|----------|
| *“Understanding what women want: eliciting preference for delivery health facility in a rural sub-County in Kenya, a discrete choice experiment”* – Oluoch-Aridi et al., 2020, Dryad repository. DOI: 10.5061/dryad.1vhhmgqrk :contentReference[oaicite:9]{index=9} |

The original Excel file (`finalproject.xlsx`, sheet **Naivasha database**) contains 39 columns and 22 368 rows :contentReference[oaicite:10]{index=10}.  
A lightweight, anonymised CSV (`cleaned_data.csv`) with only the variables listed above is provided for rapid experimentation.

---

## 3. Repository structure

