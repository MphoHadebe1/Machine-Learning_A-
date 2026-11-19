# CSC2042S Assignment 3: Neural Networks

Mpho Hadebe| HDBMPH001

This is my submission for Assignment 3. I train a small MLP (784-128-64-10) on Fashion-MNIST in PyTorch, use its 10-epoch validation accuracy as the baseline, then tune three hyperparameters to try to beat it. The notebook has the code and the report has the analysis.

## Files

- `HDBMPH001_Assignment3.ipynb`: all the code, from data loading through to the results table, plots and confusion matrix.
- `HDBMPH001_report.pdf`: the report (5 pages max), with my design decisions, results, interpretation and AI usage statement.
- `README.md`: this file.
- `.git`: git repository


I haven't included any data. The dataset downloads itself when you run the notebook.

## Setup

You need Python and these packages: torch, torchvision, numpy, pandas, matplotlib, scikit-learn.

```bash
python -m venv venv
source venv/bin/activate      # Windows: venv\Scripts\activate
pip install torch torchvision numpy pandas matplotlib scikit-learn
jupyter notebook
```

It also runs on Google Colab with no setup.

## Running it

Open the notebook and use Restart & Run All. The first run needs internet so torchvision can download Fashion-MNIST into `./data`. The 60,000 training images are split 50,000 for training and 10,000 for validation, and everything is normalised.

The whole thing takes about 141 minutes on CPU. I set the random seed to [42], but results can still shift a little between machines.



## Sources

- Xiao, Rasul and Vollgraf (2017), Fashion-MNIST, Zalando Research
- PyTorch docs: https://pytorch.org/docs/


## AI use

Declared in the AI usage statement at the end of the report.
