# Machine Learning Tutorials (Jupyter Notebooks) — English & فارسی

A bilingual, notebook-first machine learning course delivered in **Jupyter Notebook (`.ipynb`)** format.  
Each lesson is provided in:

- **English**: `Tutorials/English/...`
- **Persian (Farsi / فارسی)**: `Tutorials/Persian/...` (files end with `_Fa.ipynb`)

The English and Persian notebooks cover the **same material**, with the Persian version being a translation of the English content.

---

## Repository layout

```
Datasets/
  Classification/   # tabular datasets for classification examples
  Regression/       # tabular datasets for regression examples
  Clustering/       # datasets for unsupervised learning and clustering
Tutorials/
  English/
    Chapter1/
      Chapter1_Lesson1.ipynb
      Chapter1_Lesson2.ipynb
      ...
    ...
    Chapter37/
      Chapter37_Lesson1.ipynb
      Chapter37_Lesson2.ipynb
      ...
  Persian/
    Chapter1/
      Chapter1_Lesson1_Fa.ipynb
      Chapter1_Lesson2_Fa.ipynb
      ...
    ...
    Chapter37/
      Chapter37_Lesson1_Fa.ipynb
      Chapter37_Lesson2_Fa.ipynb
      ...
css/
  rtl.css           # RTL styles used by Persian notebooks
```

- **Datasets/** contains CSV files used in examples, exercises, and projects.
- **Tutorials/** contains the notebooks organized by **Chapter → Lesson**.
- **css/rtl.css** supports right-to-left rendering (Persian) and related typography.

---

## What you will learn (high-level)

This course spans an end-to-end classical machine learning curriculum, progressing from fundamentals to advanced topics and applied case studies:

- **Foundations**: what ML is, problem framing, learning paradigms, workflow, and reproducibility concepts.
- **Data & preprocessing**: data types, cleaning, missing data, encoding, scaling, feature engineering, leakage prevention, and pipeline hygiene.
- **EDA and diagnostics**: visualization, correlation and relationships, hypothesis testing in ML context, reporting, and practical data-quality forensics.
- **Supervised learning**: regression and classification, linear/logistic models, regularization, GLMs, multiclass/ordinal settings, robust methods, and cost-sensitive decisioning.
- **Tree-based learning**: CART and related algorithms, pruning, interpretability, feature importance, and practical concerns (missing/categorical handling, stability).
- **Ensembles**: bagging, boosting, stacking, calibration, imbalance handling, and modern gradient boosting families (including advanced tuning and interpretability ideas).
- **Kernel & instance-based methods**: kNN, distance metrics, curse of dimensionality, metric learning overview, and kernel methods beyond SVM.
- **Probabilistic modeling**: Naïve Bayes variants, Bayesian perspectives, priors/MAP, and EM intuition.
- **Unsupervised learning**: clustering families (k-means, hierarchical, mixtures, density-based, spectral) plus evaluation and stability concepts.
- **Dimensionality reduction**: PCA, t-SNE, LDA, ICA, NMF, random projections, and embedded feature selection.
- **Model evaluation**: cross-validation strategies, calibration, learning curves, nested CV, uncertainty in metrics, and decision analysis.
- **Time series**: classical forecasting workflows, ARIMA/Prophet concepts, proper CV, feature engineering, and anomaly/event detection fundamentals.
- **Reliability & uncertainty**: calibration, prediction intervals, conformal prediction basics, and shift-aware evaluation.
- **Responsible ML**: fairness, privacy, robustness, and security considerations for classical ML systems.
- **MLOps (classical)**: experiment tracking concepts, versioning, deployment patterns, monitoring, governance, and maintenance practices.
- **Capstone projects**: end-to-end, notebook-driven projects across classification, regression with uncertainty, clustering/segmentation, forecasting, anomaly detection, and causal/uplift thinking.

---

## Getting started

### 1) Install Python (recommended)
- Install **Python 3.9+** (or a newer 3.x release).
- Recommended option for data science workflows: **Anaconda / Miniconda**.

### 2) Install Jupyter (Windows / macOS / Linux)

#### Option A — Install via pip (works on all platforms)
```bash
python -m pip install --upgrade pip
python -m pip install notebook jupyterlab
```

Then launch:
```bash
jupyter lab
# or
jupyter notebook
```

#### Option B — Install via conda (recommended if you use Anaconda/Miniconda)
```bash
conda install -c conda-forge notebook jupyterlab
```

Then launch:
```bash
jupyter lab
# or
jupyter notebook
```

### 3) Install course dependencies (requrement.txt)

This repository includes a **`requrement.txt`** file (intentionally kept as the repo’s dependency manifest).  
It lists the **Python packages used throughout the notebooks** (NumPy, Pandas, Matplotlib, SciPy, scikit-learn, and supporting tools).

#### Option A — Create a virtual environment (recommended) and install with pip

From the repository root:

```bash
# Create a virtual environment
python -m venv .venv

# Activate it (Windows PowerShell)
.venv\Scripts\Activate.ps1

# Activate it (Windows CMD)
.venv\Scripts\activate.bat

# Activate it (macOS/Linux)
source .venv/bin/activate

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
python -m pip install -r requrement.txt
```

Then start Jupyter from the repo root:
```bash
jupyter lab
# or
jupyter notebook
```

#### Option B — Use conda and install with pip

```bash
conda create -n ml-tutorials python=3.11
conda activate ml-tutorials
python -m pip install --upgrade pip
python -m pip install -r requrement.txt
```

---

## Download / clone the repository

### Download as ZIP
1. Click **Code → Download ZIP** on GitHub.
2. Extract the ZIP file to a local folder.

### Clone with Git
```bash
git clone https://github.com/<YOUR-USERNAME>/<YOUR-REPO>.git
cd <YOUR-REPO>
```

---

## Open notebooks so only this repo appears

To ensure Jupyter shows **only the files/folders inside this repository**, start Jupyter from the repo root directory.

### JupyterLab (recommended)
```bash
cd <YOUR-REPO>
jupyter lab
```

### Jupyter Notebook (classic)
```bash
cd <YOUR-REPO>
jupyter notebook
```

#### (Optional) Force notebook root explicitly
If you want to be explicit about the working directory:
```bash
cd <YOUR-REPO>
jupyter notebook --notebook-dir="."
```

From the file browser, navigate to:
- `Tutorials/English/ChapterX/` for English notebooks
- `Tutorials/Persian/ChapterX/` for Persian notebooks (`*_Fa.ipynb`)

---

## Important: run the first cell first (CSS + RTL + fonts)

In **each notebook**, the **first cell** is responsible for applying display styling (for example, loading CSS for right-to-left layout and fonts for Persian).  

Before reading or executing anything else:
1. Open the notebook
2. **Run the first cell**
3. Continue with the remaining lesson cells

This ensures the Persian notebooks render correctly and consistently.

---

## YouTube walkthrough

A short video walkthrough shows how to download/clone the repo and run the notebooks.

<a href="https://www.youtube.com/watch?v=HwZptWXj4pA" target="_blank">
  <img
    src="https://i.ytimg.com/vi/HwZptWXj4pA/maxresdefault.jpg"
    alt="ODE/PDE in C# - Implementation Tutorial"
    style="max-width: 100%; border-radius: 10px; box-shadow: 0 6px 18px rgba(0,0,0,0.18); margin-top: 0.5rem;"
  />
</a>
