# CSC2042S Assignment 2 — Multinomial Logistic Regression for Multilingual News Classification

**Student Number:** HDBMPH001

## 1. Overview

This project implements multinomial logistic regression for multilingual news topic classification using the MasakhaNEWS dataset. The model classifies news articles in English, isiXhosa, and chiShona using Binary Bag-of-Words, Count Bag-of-Words, and TF-IDF feature representations.

## 2. Repository Structure

```text
├── Assignment2.ipynb
├── REPORT_A2.pdf
└── README.md
```

All implementation, training, experiments, and evaluation are contained in the Jupyter notebook.

## 3. Setup Instructions

The project was developed using Python 3.13.

The following Python libraries are required:

- PyTorch
- pandas
- NumPy
- scikit-learn
- matplotlib

Install the required libraries using:

```bash
pip install torch pandas numpy scikit-learn matplotlib
```

The MasakhaNEWS dataset is not included in the submission. Place the dataset in the following directory structure relative to the notebook:

```text
../news-dataset/news-dataset/
├── eng/
│   ├── train.tsv
│   ├── dev.tsv
│   └── test.tsv
├── xho/
│   ├── train.tsv
│   ├── dev.tsv
│   └── test.tsv
└── sna/
    ├── train.tsv
    ├── dev.tsv
    └── test.tsv
```

Each language directory must contain its corresponding training, development, and test TSV files.

## 4. How to Run

1. Install the required Python libraries.
2. Place the MasakhaNEWS dataset in the directory structure shown above.
3. Open `Assignment2.ipynb` using Jupyter Notebook or VS Code.
4. Run the notebook cells from top to bottom.

A fixed random seed of `42` is used for reproducibility.

The notebook runs the complete workflow, including preprocessing, feature extraction, model training, hyperparameter tuning, class-imbalance experiments, bilingual training, and evaluation.

## 5. File-by-File Description

- `Assignment2.ipynb` — Main notebook containing data loading, preprocessing, feature extraction, multinomial logistic regression implementation, training, hyperparameter tuning, class-imbalance experiments, bilingual training, and model evaluation.

- `CSC2042S_A2_REPORT.pdf` — Final report containing the methodology, experimental results, analysis, and conclusions.

- `README.md` — Contains the project overview, setup instructions, running instructions, and descriptions of the submitted files.

## 6. Notes / Known Limitations

The hyperparameter tuning sections train multiple model configurations across the three languages and feature representations and may therefore take longer to run than the other sections of the notebook.

The dataset is not included in the repository and must be placed in the expected directory before running the notebook.
