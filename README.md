# CMPS 460 Machine Learning Project - G2 TCGA-CHOL

This project contains a completed Jupyter Notebook for binary cancer classification using the assigned TCGA-CHOL gene expression dataset.

## Files

```text
ML_Project/
├─ CMPS460_G2_CHOL_Final_Project.ipynb
├─ CMPS460-Project.pdf
├─ requirements.txt
├─ README.md
├─ outputs/
│  ├─ figures/
│  └─ tables/
└─ data/
   ├─ G2-TCGA-CHOL_EX.csv
   └─ G2-TCGA-CHOL_Label.csv
```

## Setup on Windows

```powershell
cd "PATH\ML_Project"
python -m venv .venv
.\.venv\Scripts\activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
jupyter notebook
```

Open `CMPS460_G2_CHOL_Final_Project.ipynb` and run all cells from top to bottom.

## Important data note

The uploaded CSV files do **not** have header rows. The final notebook checks this before loading and treats the files as headerless numeric CSVs.

## What the final notebook includes

- Dataset explanation based on the project PDF
- Exploratory data analysis with saved figures and tables
- Leakage-safe preprocessing with stratified split, scaling, and `SelectKBest`
- Logistic Regression, Random Forest, and neural-network models
- Baseline and optimized model comparison
- Feature ranking and final discussion preparation

TensorFlow is optional. If TensorFlow/Keras is unavailable, the notebook uses `sklearn.neural_network.MLPClassifier` as the fallback deep learning model.
