# Machine Learning Tutorials (Jupyter Notebooks) — English & فارسی

A bilingual, notebook-first machine learning course delivered in **Jupyter Notebook (`.ipynb`)** format. The repository is designed as a structured, chapter-by-chapter curriculum for learners who want a practical and theoretical path through classical machine learning, model evaluation, time series, reliability, MLOps, and applied case studies.

Each lesson is provided in:

- **English**: `Tutorials/English/...`
- **Persian (Farsi / فارسی)**: `Tutorials/Persian/...` with Persian notebooks ending in `_Fa.ipynb`

The English and Persian notebooks cover the same material, with the Persian version being a translation of the English content.

---

## Repository layout

```text
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
- **css/rtl.css** supports right-to-left rendering for Persian notebooks.

---

## Course size

This curriculum contains:

- **37 chapters**
- **330 lessons**
- Introductory, advanced, and comprehensive extension modules
- End-to-end capstone projects for applied classical machine learning

---

## What you will learn

This course spans an end-to-end classical machine learning curriculum, progressing from foundations to advanced topics and applied case studies:

- Machine learning foundations, problem formulation, workflow design, and reproducibility
- Data preprocessing, feature engineering, leakage prevention, and pipeline hygiene
- Exploratory data analysis, diagnostics, statistical testing, and data-quality forensics
- Supervised learning: regression, classification, GLMs, regularization, robust methods, and cost-sensitive learning
- Decision trees, tree variants, ensemble learning, boosting, calibration, and imbalanced learning
- SVMs, kernel methods, instance-based learning, and probabilistic models
- Unsupervised learning, clustering, dimensionality reduction, and association rules
- Cross-validation, model evaluation, uncertainty estimation, and decision analysis
- Time series modeling, forecasting, rolling validation, and anomaly detection
- Bayesian networks, graphical models, Gaussian processes, causal inference, and experimentation
- Fairness, privacy, robustness, security, reliability, conformal prediction, and MLOps
- Scalable, online, specialized, and capstone machine learning workflows

---

## Full course curriculum

# Introductory Course of Machine Learning

## Chapter 1: Introduction to Machine Learning

- Lesson 1: What is Machine Learning?
- Lesson 2: Types of Machine Learning (Supervised, Unsupervised, Semi-Supervised, Reinforcement Learning)
- Lesson 3: Applications and Real-World Use Cases
- Lesson 4: ML Workflow (Data, Model, Evaluation, Deployment)
- Lesson 5: History and Evolution of ML
- Lesson 6: Key Mathematical Foundations (Linear Algebra, Probability, Optimization)
- Lesson 7: Common Misconceptions and Challenges in ML
- Lesson 8: ML vs. Statistics vs. Data Mining vs. AI (Boundaries and Overlaps)
- Lesson 9: Problem Formulation (Inputs/Outputs, Objective, Constraints, Costs)
- Lesson 10: Learning Paradigms and Task Taxonomy (Regression, Classification, Ranking, Forecasting)
- Lesson 11: What “Good Performance” Means (Generalization, Robustness, Reliability)
- Lesson 12: Reproducibility Basics (Random Seeds, Determinism, Experiment Tracking Concepts)

## Chapter 2: Basics of Data and Preprocessing

- Lesson 1: Understanding Data Types and Structures
- Lesson 2: Data Cleaning and Missing Values
- Lesson 3: Data Transformation and Encoding
- Lesson 4: Feature Scaling (Normalization & Standardization)
- Lesson 5: Handling Outliers and Imbalanced Data
- Lesson 6: Feature Engineering Fundamentals
- Lesson 7: Data Leakage and Prevention Techniques
- Lesson 8: Data Collection and Label Quality (Noise, Ambiguity, Measurement Error)
- Lesson 9: Missingness Mechanisms (MCAR, MAR, MNAR) and Practical Implications
- Lesson 10: Imputation Methods (Simple, kNN, Iterative/Multiple Imputation Concepts)
- Lesson 11: Encoding Categorical Features (One-Hot, Ordinal, Hashing, Target Encoding)
- Lesson 12: Train/Validation/Test Hygiene (Temporal Splits, Group Splits, Entity Leakage)
- Lesson 13: Building Preprocessing Pipelines (Fit/Transform Discipline, Column-Wise Pipelines)

## Chapter 3: Exploratory Data Analysis (EDA)

- Lesson 1: Visualizing Data Distributions
- Lesson 2: Pairwise Relationships (Correlation, Scatterplots)
- Lesson 3: Detecting Patterns in Data
- Lesson 4: Dimensionality Reduction (Intro to PCA)
- Lesson 5: Using Tools like Pandas, Matplotlib, and Seaborn
- Lesson 6: Statistical Hypothesis Testing in ML Context
- Lesson 7: EDA for Data Quality (Duplicates, Inconsistencies, Drift, Label Issues)
- Lesson 8: Multicollinearity and Confounding Signals (Detection and Mitigation)
- Lesson 9: Leakage Forensics in EDA (Suspicious Features, Post-Outcome Variables)
- Lesson 10: EDA Reporting (Narratives, Assumptions, and Actionable Insights)

## Chapter 4: Supervised Learning Basics

- Lesson 1: Introduction to Regression and Classification
- Lesson 2: Linear Regression: Concept and Applications
- Lesson 3: Logistic Regression: Binary Classification
- Lesson 4: Overfitting and Regularization (Ridge, LASSO, Elastic Net)
- Lesson 5: All Model Evaluation Metrics (MAE, MSE, RMSE, Accuracy, etc.)
- Lesson 6: Bias-Variance Tradeoff and Model Complexity
- Lesson 7: Polynomial and Interaction Terms in Regression Models
- Lesson 8: Generalized Linear Models (GLMs) Overview (Link Functions, Likelihood)
- Lesson 9: Multiclass Logistic Regression (Softmax) and Evaluation
- Lesson 10: Ordinal Regression (When Class Order Matters)
- Lesson 11: Robust Regression (Huber, RANSAC Concepts and Use Cases)
- Lesson 12: Quantile Regression and Prediction Intervals (Intro)
- Lesson 13: Cost-Sensitive Learning Basics (Thresholding, Costs, Utility)

## Chapter 5: Decision Trees and Variants

- Lesson 1: Concept of Decision Trees
- Lesson 2: CART (Classification and Regression Trees)
- Lesson 3: Pruning and Overfitting in Trees
- Lesson 4: CHAID and M5 Model Trees
- Lesson 5: C4.5 and C5.0 Decision Trees
- Lesson 6: Interpretability and Feature Importance in Trees
- Lesson 7: Split Criteria (Gini, Entropy, Gain Ratio, Variance Reduction)
- Lesson 8: Handling Missing Values and Categorical Variables in Trees
- Lesson 9: Tree Stability, Variance, and Sensitivity Analysis
- Lesson 10: Monotonic Constraints and Business Rules in Tree Models (Concepts)

## Chapter 6: Ensemble Learning Techniques

- Lesson 1: What is Ensemble Learning?
- Lesson 2: Bagging Algorithms (Random Forest, Bootstrap Aggregation)
- Lesson 3: Boosting Algorithms (AdaBoost, Gradient Boosting)
- Lesson 4: Stacking and Blending Techniques
- Lesson 5: Comparison of Ensemble Methods
- Lesson 6: Voting Classifiers and Averaging Methods
- Lesson 7: Bias-Variance Reduction via Ensembles
- Lesson 8: Out-of-Bag (OOB) Estimation and When It Works
- Lesson 9: Extremely Randomized Trees (ExtraTrees) and Diversity
- Lesson 10: Calibration with Ensembles (Platt Scaling, Isotonic Regression Overview)
- Lesson 11: Imbalanced Data with Ensembles (Class Weights, Balanced RF, Thresholding)

## Chapter 7: Support Vector Machines (SVM)

- Lesson 1: Concept of SVM for Classification
- Lesson 2: Kernel Functions in SVM
- Lesson 3: Soft Margin and Hyperparameters
- Lesson 4: Support Vector Regression (SVR)
- Lesson 5: Applications of SVM in Real-World Problems
- Lesson 6: Mathematical Formulation of the SVM Optimization Problem
- Lesson 7: Kernel Trick Intuition and Feature Spaces
- Lesson 8: Multi-Class SVM Strategies (OvR, OvO) and Practical Tradeoffs
- Lesson 9: SVM Probability Estimates and Calibration Considerations
- Lesson 10: Scaling SVMs (Approximate Kernels, Linear SVMs, Complexity)

## Chapter 8: Instance-Based Learning

- Lesson 1: K-Nearest Neighbors (KNN) Algorithm
- Lesson 2: Choosing the Right K
- Lesson 3: Distance Metrics and Weighting
- Lesson 4: Locally Weighted Learning (LWL)
- Lesson 5: Applications and Challenges
- Lesson 6: Curse of Dimensionality and Its Impact on KNN
- Lesson 7: kNN Regression and Local Smoothing Bias/Variance
- Lesson 8: Approximate Nearest Neighbors (KD-Trees, Ball Trees, ANN Concepts)
- Lesson 9: Metric Learning Overview (When Distances Should Be Learned)

## Chapter 9: Probabilistic Models

- Lesson 1: Naïve Bayes Classifier
- Lesson 2: Gaussian Naïve Bayes
- Lesson 3: Bayesian Linear Regression
- Lesson 4: Assumptions and Limitations
- Lesson 5: Case Studies with Probabilistic Models
- Lesson 6: Maximum Likelihood vs. Bayesian Estimation
- Lesson 7: Bayesian Decision Theory (Risk, Loss, Bayes Optimal Classifier)
- Lesson 8: Priors and Conjugacy (Conceptual Toolkit for Fast Bayesian Updates)
- Lesson 9: MAP Estimation, Regularization Connections, and Interpretations
- Lesson 10: Expectation-Maximization (EM) Intuition (Preview for Later Chapters)

## Chapter 10: Unsupervised Learning Basics

- Lesson 1: Introduction to Clustering
- Lesson 2: K-Means Clustering
- Lesson 3: Hierarchical Clustering
- Lesson 4: Gaussian Mixture Models (GMM)
- Lesson 5: Applications of Clustering Techniques
- Lesson 6: Evaluation Metrics for Clustering (Silhouette, Davies-Bouldin)
- Lesson 7: K-Means Variants (k-medoids, k-means++ initialization)
- Lesson 8: Model-Based Clustering and Selecting Number of Clusters (AIC/BIC concepts)
- Lesson 9: Constraints and Practicalities (Must-Link/Cannot-Link, Business Constraints)
- Lesson 10: Clustering at Scale (Mini-Batch K-Means and Sampling Strategies)

## Chapter 11: Dimensionality Reduction

- Lesson 1: Principal Component Analysis (PCA)
- Lesson 2: t-SNE for Visualization
- Lesson 3: Linear Discriminant Analysis (LDA)
- Lesson 4: Feature Selection vs Feature Extraction
- Lesson 5: Applications of Dimensionality Reduction
- Lesson 6: Independent Component Analysis (ICA)
- Lesson 7: Random Projections and Johnson–Lindenstrauss Intuition
- Lesson 8: Non-negative Matrix Factorization (NMF) for Parts-Based Representations
- Lesson 9: Sparse PCA and Interpretability Tradeoffs
- Lesson 10: Embedded Feature Selection (L1, Tree-Based, Permutation Importance Overview)

## Chapter 12: Association Rule Learning

- Lesson 1: Concept of Association Rules
- Lesson 2: Apriori Algorithm
- Lesson 3: Eclat Algorithm
- Lesson 4: Market Basket Analysis
- Lesson 5: Challenges and Limitations
- Lesson 6: Evaluation Metrics (Support, Confidence, Lift)
- Lesson 7: FP-Growth (Frequent Pattern Growth) and When It Outperforms Apriori
- Lesson 8: Rule Pruning and Redundancy Control
- Lesson 9: Sequential Pattern Mining (Concepts and Use Cases)

## Chapter 13: Cross-Validation and Model Evaluation

- Lesson 1: Train-Test Split and Validation
- Lesson 2: K-Fold Cross-Validation
- Lesson 3: Stratified Sampling in Cross-Validation
- Lesson 4: Performance Metrics for Classification
- Lesson 5: Performance Metrics for Regression
- Lesson 6: Model Calibration and ROC Curves
- Lesson 7: Learning Curves and Validation Curves
- Lesson 8: Nested Cross-Validation for Model Selection (Leakage Avoidance)
- Lesson 9: Bootstrap Methods for Performance Estimation and Uncertainty
- Lesson 10: Statistical Tests for Comparing Models (Paired Tests, Practical Significance)
- Lesson 11: Threshold Tuning and Decision Analysis (Costs, Utility, Decision Curves)
- Lesson 12: Confidence Intervals for Metrics and Reporting Standards

## Chapter 14: Time Series Analysis Basics

- Lesson 1: Introduction to Time Series Data
- Lesson 2: ARIMA Model
- Lesson 3: Decomposition and Seasonal Patterns
- Lesson 4: Dynamic Time Warping
- Lesson 5: Prophet for Time Series Forecasting
- Lesson 6: Feature Engineering for Time Series ML Models
- Lesson 7: Stationarity, ACF/PACF, and Differencing Practicalities
- Lesson 8: Time Series Cross-Validation (Rolling/Expanding Windows)
- Lesson 9: Forecast Accuracy Metrics (MAPE/sMAPE/MASE, Horizon-Based Evaluation)
- Lesson 10: Exogenous Variables and Feature Lags (ARIMAX/Regression with Lags Concepts)
- Lesson 11: Change Points and Regime Shifts (Introductory Concepts)

# Advanced Course of Machine Learning

## Chapter 15: Advanced Ensemble Methods

- Lesson 1: XGBoost: Concepts and Implementation
- Lesson 2: LightGBM and CatBoost
- Lesson 3: Advanced Hyperparameter Tuning in Boosting
- Lesson 4: Comparison of Gradient Boosting Variants
- Lesson 5: Applications and Limitations
- Lesson 6: Interpretability and SHAP Values in Boosting Models
- Lesson 7: Regularization and Constraints in Gradient Boosting (Shrinkage, Depth, Monotonicity)
- Lesson 8: Handling Categorical Variables and Missingness in Modern GBDTs (Conceptual + Practical)
- Lesson 9: Robustness, Leakage, and Validation Pitfalls in Boosted Models

## Chapter 16: Semi-Supervised and Active Learning

- Lesson 1: Introduction to Semi-Supervised Learning
- Lesson 2: Self-Training and Co-Training Approaches
- Lesson 3: Active Learning for Data Labeling
- Lesson 4: Applications of Semi-Supervised Learning
- Lesson 5: Case Studies
- Lesson 6: Label Propagation and Graph-Based Semi-Supervised Learning
- Lesson 7: Query Strategies (Uncertainty Sampling, Diversity Sampling, Expected Model Change)
- Lesson 8: Evaluation Protocols for Active Learning (Budget Curves, Label Noise, Stopping Rules)
- Lesson 9: Weak Supervision and Silver Labels (Concepts, Risks, Governance)

## Chapter 17: Advanced Clustering Techniques

- Lesson 1: Density-Based Clustering (DBSCAN)
- Lesson 2: Mean Shift Clustering
- Lesson 3: Spectral Clustering
- Lesson 4: Fuzzy C-Means Clustering
- Lesson 5: Comparison of Advanced Clustering Algorithms
- Lesson 6: Performance Metrics for Clustering
- Lesson 7: Cluster Stability and Validation Techniques
- Lesson 8: OPTICS and HDBSCAN (Variable Density Clustering Concepts)
- Lesson 9: Clustering High-Dimensional Data (Distance Concentration, Subspace Methods Overview)
- Lesson 10: Clustering Streams and Incremental Updates (Concepts)

## Chapter 18: Bayesian Networks and Probabilistic Graphical Models

- Lesson 1: Introduction to Bayesian Networks
- Lesson 2: Markov Random Fields
- Lesson 3: Conditional Random Fields
- Lesson 4: Applications in Real-World Problems
- Lesson 5: Challenges in Building Bayesian Models
- Lesson 6: Structure Learning and Inference Algorithms
- Lesson 7: Exact Inference (Variable Elimination) vs Approximate Inference (Sampling/Variational)
- Lesson 8: Belief Propagation and Message Passing Intuition
- Lesson 9: Parameter Learning with EM in Graphical Models

## Chapter 19: Advanced Time Series Models

- Lesson 1: Long-Term Forecasting Techniques
- Lesson 2: Prophet in Depth
- Lesson 3: Regularization in Time Series
- Lesson 4: Dynamic Time Warping for Sequence Alignment
- Lesson 5: Use Cases in Finance and Healthcare
- Lesson 6: ML-Based Time Series Models (Random Forest, XGBoost, SVR)
- Lesson 7: State Space Models and Kalman Filtering (Conceptual + Practical)
- Lesson 8: Volatility and Heteroskedasticity (ARCH/GARCH Concepts)
- Lesson 9: Hierarchical and Grouped Forecasting (Reconciliation Concepts)
- Lesson 10: Conformal Prediction for Forecast Uncertainty (Intro)
- Lesson 11: Anomaly Detection and Event Detection in Time Series (Classical Methods)

## Chapter 20: Transformers and Variants

- Lesson 1: Introduction to Transformer Models
- Lesson 2: Applications of Transformers in ML
- Lesson 3: Vision Transformers (ViT)
- Lesson 4: Comparing Transformers with Traditional Methods
- Lesson 5: Advanced Research Trends
- Lesson 6: Transfer Learning and Fine-Tuning Principles
- Lesson 7: Conceptual Positioning (Why Transformers Are Typically Considered Deep Learning)
- Lesson 8: Classical Alternatives for Sequences (HMMs, State Space, DTW, Feature-Based Models)

## Chapter 21: Regularization Techniques

- Lesson 1: Advanced Regularization (Elastic Net, etc.)
- Lesson 2: L1 and L2 Regularization in Depth
- Lesson 3: Impact of Regularization on Overfitting
- Lesson 4: Applications in Sparse Data
- Lesson 5: Case Studies
- Lesson 6: Dropout and Noise-Based Regularization (General ML Perspective)
- Lesson 7: Regularization Paths and Model Selection (Lambda Grids, Warm Starts)
- Lesson 8: Group Lasso, Fused Lasso, and Structured Sparsity (Overview)
- Lesson 9: Regularization Beyond Linear Models (Trees/Boosting Constraints, Early Stopping)

## Chapter 22: Hyperparameter Optimization

- Lesson 1: Grid Search and Random Search
- Lesson 2: Bayesian Optimization
- Lesson 3: Genetic Algorithms for Optimization
- Lesson 4: Tuning Models with Optuna
- Lesson 5: Best Practices in Hyperparameter Tuning
- Lesson 6: Early Stopping and Learning Rate Scheduling
- Lesson 7: Multi-Fidelity Optimization (Successive Halving, Hyperband Concepts)
- Lesson 8: Parallel and Distributed HPO (Practical Patterns and Failure Modes)
- Lesson 9: Search Space Design (Priors, Conditional Spaces, Constraints, and Budgets)

## Chapter 23: Emerging Topics in ML

- Lesson 1: Explainable AI (XAI)
- Lesson 2: Fairness and Bias in Machine Learning
- Lesson 3: Ethical Considerations in ML Models
- Lesson 4: Automated Machine Learning (AutoML)
- Lesson 5: Research Directions in ML
- Lesson 6: Model Compression and Distillation
- Lesson 7: Continual and Lifelong Learning in ML
- Lesson 8: Data-Centric AI (Systematic Data Improvement, Label Governance)
- Lesson 9: Conformal Prediction and Reliability Guarantees (Survey)
- Lesson 10: Privacy-Preserving ML (Differential Privacy Concepts)
- Lesson 11: Federated Learning (Non-Deep Learning Perspective, Constraints and Tradeoffs)
- Lesson 12: Robust ML and Distribution Shift (OOD, Stress Testing, Robustness Curves)
- Lesson 13: Adversarial ML for Classical Models (Poisoning, Evasion, Threat Modeling)

# Added Chapters to Make the Course Comprehensive

## Chapter 24: Optimization for Machine Learning

- Lesson 1: Optimization Problem Setup (Objectives, Constraints, Regularizers)
- Lesson 2: Convexity, Strong Convexity, and Why They Matter
- Lesson 3: Gradient Descent, SGD, Momentum (Classical View)
- Lesson 4: Newton, Quasi-Newton (BFGS/L-BFGS) and Second-Order Intuition
- Lesson 5: Coordinate Descent and Proximal Methods (L1/Lasso Context)
- Lesson 6: Duality and KKT Conditions (SVM/Regularization Connections)
- Lesson 7: Numerical Stability, Conditioning, and Practical Debugging

## Chapter 25: Statistical Learning Theory

- Lesson 1: Generalization Error and Concentration Intuition
- Lesson 2: VC Dimension (Conceptual) and Capacity Measures
- Lesson 3: PAC Learning (High-Level) and Sample Complexity
- Lesson 4: Regularization as Capacity Control
- Lesson 5: Bias-Variance Revisited Through Theory
- Lesson 6: No Free Lunch Theorems and Practical Implications

## Chapter 26: Model Selection and Feature Selection in Depth

- Lesson 1: Model Selection vs Hyperparameter Tuning vs Statistical Inference
- Lesson 2: Filter Methods (Mutual Information, Chi-Square, ANOVA F-test)
- Lesson 3: Wrapper Methods (RFE, Forward/Backward Selection) and Costs
- Lesson 4: Embedded Methods (L1, Trees, Stability Selection Concepts)
- Lesson 5: Permutation Importance and Pitfalls (Correlation, Leakage, Variance)
- Lesson 6: Multiple Comparisons and Selection Bias (Why Results Look Too Good)
- Lesson 7: Parsimony, Interpretability, and Governance Requirements

## Chapter 27: Kernel Methods Beyond SVM

- Lesson 1: Kernels as Similarity Functions (Design and Validity)
- Lesson 2: Kernel Ridge Regression and Regularization
- Lesson 3: Kernel PCA and Nonlinear Manifolds
- Lesson 4: Approximate Kernels (Nyström, Random Fourier Features)
- Lesson 5: Choosing Kernels and Tuning in Practice
- Lesson 6: When Kernel Methods Beat Trees (and When They Don’t)

## Chapter 28: Gaussian Processes for Regression and Classification

- Lesson 1: GP Intuition (Distributions over Functions)
- Lesson 2: Covariance Functions (RBF, Matérn, Periodic) and Prior Beliefs
- Lesson 3: Hyperparameter Learning (Marginal Likelihood)
- Lesson 4: Uncertainty Quantification and Prediction Intervals
- Lesson 5: Scalability (Sparse GPs, Inducing Points Concepts)
- Lesson 6: GP Classification (Laplace/Variational Ideas at a High Level)
- Lesson 7: Practical Use Cases and Limitations

## Chapter 29: Anomaly Detection and Novelty Detection

- Lesson 1: Problem Definitions (Outliers vs Anomalies vs Novelty)
- Lesson 2: Statistical Methods (Z-score, Robust Covariance, MAD)
- Lesson 3: Density-Based Methods (GMM-Based, KDE Concepts)
- Lesson 4: Isolation Forest and Tree-Based Anomaly Detection
- Lesson 5: One-Class SVM and Support Estimation
- Lesson 6: Local Outlier Factor (LOF) and Neighborhood Methods
- Lesson 7: Evaluation Without Labels (Proxy Metrics, Triage Workflows)

## Chapter 30: Recommendation Systems and Ranking (Classical)

- Lesson 1: Recommendation Problem Types (Explicit vs Implicit Feedback)
- Lesson 2: Baselines and Heuristics (Popularity, Co-Occurrence, Rules)
- Lesson 3: Collaborative Filtering (User–User, Item–Item)
- Lesson 4: Matrix Factorization (SVD/ALS Concepts)
- Lesson 5: Content-Based Recommendation (Feature Engineering)
- Lesson 6: Ranking Metrics (NDCG, MAP, Recall@K) and Offline Evaluation
- Lesson 7: Cold Start, Leakage, and Serving-Time Constraints

## Chapter 31: Causal Inference and Experimentation for ML Practitioners

- Lesson 1: Correlation vs Causation and Why Predictive Models Mislead
- Lesson 2: Potential Outcomes Framework (ATE, ATT Concepts)
- Lesson 3: Confounding, Selection Bias, and Backdoor Intuition
- Lesson 4: Propensity Scores (Matching, Weighting, Stratification)
- Lesson 5: Doubly Robust Estimation (High-Level) and Practical Guardrails
- Lesson 6: Uplift Modeling and Treatment Effect Heterogeneity (Conceptual)
- Lesson 7: A/B Testing Design, Power, and Common Failure Modes

## Chapter 32: Uncertainty, Reliability, and Conformal Prediction

- Lesson 1: Aleatoric vs Epistemic Uncertainty (Practical Meaning)
- Lesson 2: Calibration in Classification (Reliability Diagrams, ECE Concepts)
- Lesson 3: Prediction Intervals in Regression (Quantile Regression Linkage)
- Lesson 4: Conformal Prediction for Regression and Classification
- Lesson 5: Distribution Shift and Validity Degradation
- Lesson 6: Risk-Based Decisioning and Human-in-the-Loop Thresholds

## Chapter 33: Robustness, Fairness, Privacy, and Security (Classical ML)

- Lesson 1: Dataset Bias and Measurement Bias (Taxonomy and Examples)
- Lesson 2: Fairness Metrics (Demographic Parity, Equalized Odds, Calibration Tradeoffs)
- Lesson 3: Bias Mitigation (Pre-, In-, Post-Processing Approaches)
- Lesson 4: Privacy Concepts (PII, Re-Identification Risk, Data Minimization)
- Lesson 5: Differential Privacy Basics (Noise Mechanisms and Utility Tradeoffs)
- Lesson 6: Threat Modeling for ML Systems (Poisoning, Evasion, Model Extraction)
- Lesson 7: Secure Evaluation and Red-Teaming ML Pipelines (Process)

## Chapter 34: MLOps for Classical Machine Learning

- Lesson 1: Reproducible Pipelines (Data/Code/Model Versioning Concepts)
- Lesson 2: Feature Stores and Training/Serving Consistency
- Lesson 3: Deployment Patterns (Batch, Online, Streaming) for Classical Models
- Lesson 4: Monitoring (Data Drift, Concept Drift, Performance Decay)
- Lesson 5: Model Governance (Approvals, Documentation, Audit Trails)
- Lesson 6: Model Maintenance (Retraining Triggers, Backtesting, Rollbacks)
- Lesson 7: Experiment Tracking and Artifact Management (Practical Standards)

## Chapter 35: Scalable and Online Machine Learning

- Lesson 1: Computational Complexity in Training and Inference
- Lesson 2: Sampling, Sketching, and Approximation Concepts
- Lesson 3: Incremental/Online Learning (SGD Classifiers, Passive-Aggressive Concepts)
- Lesson 4: Streaming Feature Engineering and Windowing
- Lesson 5: Distributed Training for Classical Models (MapReduce/Spark Concepts)
- Lesson 6: Practical Performance Engineering (Vectorization, Caching, Memory Layout)

## Chapter 36: Specialized Classical ML Topics

- Lesson 1: Survival Analysis (Censoring, Kaplan–Meier, Cox Model Concepts)
- Lesson 2: Count Models (Poisson/Negative Binomial Regression Use Cases)
- Lesson 3: Multi-Label Classification (Problem Transforms, Metrics)
- Lesson 4: Imbalanced and Rare-Event Modeling (PR Curves, Focal Costs, Evaluation)
- Lesson 5: Spatial and Geospatial Modeling Basics (Leakage, Autocorrelation Concepts)
- Lesson 6: Structured Data with Groups (Hierarchical Models Concepts, Group CV)

## Chapter 37: Capstone Projects and Case Studies (Non-Deep Learning Track)

- Lesson 1: End-to-End Tabular Classification Project (From EDA to Monitoring Plan)
- Lesson 2: End-to-End Regression Project with Uncertainty (Intervals + Conformal)
- Lesson 3: Clustering and Segmentation Project (Stability + Business Interpretability)
- Lesson 4: Time Series Forecasting Project (Rolling CV + Drift Handling)
- Lesson 5: Anomaly Detection Project (Triage Workflow + Evaluation Without Labels)
- Lesson 6: Causal/Uplift Mini-Project (Policy/Intervention Decisioning)
- Lesson 7: Model Risk Review (Bias/Fairness/Privacy/Security Checklist + Documentation)

---

## Getting started

### 1. Install Python

Install **Python 3.9+** or a newer Python 3.x release.

Recommended options:

- Python from [python.org](https://www.python.org/)
- Anaconda or Miniconda for data science workflows

### 2. Install Jupyter

#### Option A — pip

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

#### Option B — conda

```bash
conda install -c conda-forge notebook jupyterlab
```

Then launch:

```bash
jupyter lab
# or
jupyter notebook
```

### 3. Install course dependencies

From the repository root, create and activate a virtual environment:

```bash
python -m venv .venv
```

Windows PowerShell:

```bash
.venv\Scripts\Activate.ps1
```

Windows CMD:

```bash
.venv\Scripts\activate.bat
```

macOS / Linux:

```bash
source .venv/bin/activate
```

Then install the required packages:

```bash
python -m pip install --upgrade pip
python -m pip install -r requirement.txt
```

---

## Download or clone the repository

### Download as ZIP

1. Open the repository page on GitHub.
2. Click **Code → Download ZIP**.
3. Extract the ZIP file to a local folder.

### Clone with Git

```bash
git clone https://github.com/mohammadijoo/Machine_Learning_Tutorials.git
cd Machine_Learning_Tutorials
```

---

## Open notebooks so only this repository appears

To ensure Jupyter shows only the files and folders inside this repository, start Jupyter from the repository root directory.

### JupyterLab

```bash
cd Machine_Learning_Tutorials
jupyter lab
```

### Jupyter Notebook classic

```bash
cd Machine_Learning_Tutorials
jupyter notebook
```

Optional explicit notebook root:

```bash
cd Machine_Learning_Tutorials
jupyter notebook --notebook-dir="."
```

From the file browser, navigate to:

- `Tutorials/English/ChapterX/` for English notebooks
- `Tutorials/Persian/ChapterX/` for Persian notebooks ending in `_Fa.ipynb`

---

## Important note for Persian notebooks

In each notebook, the first cell is responsible for applying display styling, including CSS for right-to-left layout and Persian typography.

Before reading or executing the notebook:

1. Open the notebook.
2. Run the first cell.
3. Continue with the remaining lesson cells.

This ensures that Persian notebooks render correctly and consistently.

---

## Suggested learning path

For a structured path through the repository:

1. Start with Chapters 1–4 to understand the ML workflow, data preparation, EDA, and supervised learning foundations.
2. Continue with Chapters 5–14 for trees, ensembles, SVMs, probabilistic models, unsupervised learning, model evaluation, and time series.
3. Study Chapters 15–23 for advanced model families, active learning, graphical models, regularization, HPO, XAI, fairness, and emerging topics.
4. Use Chapters 24–36 to strengthen mathematical, statistical, reliability, causal, MLOps, scalability, and specialized classical ML knowledge.
5. Finish with Chapter 37 capstone projects to practice complete end-to-end machine learning workflows.

---

## License

This project is released under the **MIT License**. See the `LICENSE` file for details.
