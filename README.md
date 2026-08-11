A collection of beginner-friendly, hands-on machine learning/deep learning  practicals for pharmaceutical sciences students. Built for classroom use in Google Colab — no prior coding experience required. 

Each notebook fetches real-world data, cleans it, builds a machine learning model, and evaluates its performance, with every code block explained in plain language.


## Few Practicals in This Repository Are:

| # | Notebook | Task Type | Algorithm | Dataset | Result |
|---|---|---|---|---|---|
| 1 | `Practical1_EGFR_Bioactivity_Regression.ipynb` | Regression | Random Forest (Morgan Fingerprints) | Live ChEMBL (EGFR, CHEMBL203) | R² = 0.74 |
| 2 | `Practical2_BreastCancer_Classification.ipynb` | Classification | Decision Tree | Breast Cancer dataset | Accuracy = 94.7% |
| 3 | `Practical3_Iris_Classification.ipynb` | Classification | K-Nearest Neighbors (KNN) | Iris Flower dataset | Accuracy = 100% |
| 4 | `Practical4_Solubility_LinearRegression.ipynb` | Regression | Linear Regression | Pharma Solubility dataset | R² = 0.906 |
| 5 | `Practical5_PimaDiabetes_Classification.ipynb` | Classification | Logistic Regression | Pima Indians Diabetes dataset | Accuracy = 74.7% |




## What You'll Learn Across These Practicals

- The difference between **regression** (predicting a number) and **classification**   (predicting a category)
- How to fetch real scientific data, either live from a public database (ChEMBL) or   from a hosted dataset (GitHub)
- Essential data cleaning steps: handling missing values, standardizing units,   removing duplicates
- How to convert raw data (chemical structures, biological/medical measurements)   into numerical features a model can learn from
- How to split data into training and testing sets, and why this matters
- How to train, evaluate, and interpret machine learning models using scikit-learn
- How to save and reuse trained models without retraining

---

## How to Use This Repository (For Students)

1. Open any notebook link above directly in GitHub — it will render with all code, explanations, and saved outputs visible.
2. To run it yourself: click **"Open in Colab"** (or manually go to [colab.research.google.com](https://colab.research.google.com) → File → Open 
   notebook → GitHub tab → paste this repository's URL).
3. Run each cell from top to bottom, in order.
4. Opening the notebook in Colab automatically creates **your own independent copy** 
   in your personal Google Drive — you can freely edit, experiment, or break things 
   without affecting this original repository.

---

## How to Use This Repository (For Reuse in Future Notebooks)

Datasets and trained models (only for EFGR practical) saved here can be loaded directly into any new Colab 
notebook without needing to re-fetch or retrain, using their raw GitHub links:

```python
import pandas as pd
df = pd.read_excel("https://raw.githubusercontent.com/drpharmacy/pharma-ml-projects/main/Excel_Files/<filename>")
```

```python
import joblib, urllib.request
urllib.request.urlretrieve("https://raw.githubusercontent.com/drpharmacy/pharma-ml-projects/main/models/<filename>.pkl", "model.pkl")
model = joblib.load("model.pkl")
```

---
