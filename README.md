# 🤖 Supervised Learning Lab — `supervized02`

<div align="center">

![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-2.x-0077B5?style=for-the-badge&logo=xgboost&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)

**A hands-on collection of supervised machine learning implementations covering classification, regression, ensemble methods, and boosting algorithms — all in clean, well-structured Jupyter Notebooks.**

</div>

---

## 📚 Table of Contents

- [Overview](#-overview)
- [Repository Structure](#-repository-structure)
- [Notebooks at a Glance](#-notebooks-at-a-glance)
- [Algorithms Covered](#-algorithms-covered)
- [Datasets Used](#-datasets-used)
- [Getting Started](#-getting-started)
- [Requirements](#-requirements)
- [Key Concepts](#-key-concepts)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🌟 Overview

`supervized02` is a curated set of Jupyter Notebooks designed to build practical intuition for **supervised machine learning** algorithms. Each notebook follows a clean pipeline:

> **Load Data → Preprocess → Train Model → Evaluate → Interpret**

Whether you're a student solidifying your ML foundations or a practitioner looking for clean reference implementations, this repo has you covered.

---

## 📁 Repository Structure

```
supervized02/
│
├── 📓 decision-tree.ipynb              # Decision Tree Classifier (Titanic)
├── 📓 decisio-tree-regressor.ipynb     # Decision Tree Regressor (Diabetes)
├── 📓 random_forest.ipynb              # Random Forest + Bagging (Titanic)
├── 📓 adaboost.ipynb                   # AdaBoost Classifier (Synthetic)
├── 📓 gradient_boosting.ipynb          # Gradient Boosting Regressor (Synthetic)
├── 📓 xgboost_classifier.ipynb         # XGBoost Classifier (Synthetic)
├── 📓 svc_implementation.ipynb         # Support Vector Classifier (Iris)
├── 📓 svr-implementaion.ipynb          # Support Vector Regressor (Diabetes)
├── 📓 hetrogenius_enseble.ipynb        # Heterogeneous Voting Ensemble
└── 📄 README.md
```

---

## 📓 Notebooks at a Glance

| # | Notebook | Algorithm | Task | Dataset |
|---|----------|-----------|------|---------|
| 1 | `decision-tree.ipynb` | Decision Tree Classifier | Classification | Titanic |
| 2 | `decisio-tree-regressor.ipynb` | Decision Tree Regressor | Regression | Diabetes |
| 3 | `random_forest.ipynb` | Random Forest + Bagging | Classification | Titanic |
| 4 | `adaboost.ipynb` | AdaBoost | Classification | Synthetic |
| 5 | `gradient_boosting.ipynb` | Gradient Boosting | Regression | Synthetic |
| 6 | `xgboost_classifier.ipynb` | XGBoost | Classification | Synthetic |
| 7 | `svc_implementation.ipynb` | Support Vector Classifier | Classification | Iris |
| 8 | `svr-implementaion.ipynb` | Support Vector Regressor | Regression | Diabetes |
| 9 | `hetrogenius_enseble.ipynb` | Voting Ensemble (LR + SVC + DT) | Classification | Synthetic |

---

## 🧠 Algorithms Covered

### 🌳 Tree-Based Models
- **Decision Tree Classifier** — Feature importance, tree visualization with `plot_tree`, handling missing values with `SimpleImputer`, and `LabelEncoder` for categorical features.
- **Decision Tree Regressor** — Depth-tuned regression tree on continuous targets, with MSE evaluation.

### 🌲 Ensemble Methods
- **Random Forest** — Out-of-bag (OOB) scoring, 501-estimator forest, comparison against a single Decision Tree baseline.
- **Bagging Classifier** — Bootstrap aggregation over Decision Tree base learners.
- **Voting Classifier** *(Heterogeneous Ensemble)* — Combines Logistic Regression, SVC, and Decision Tree via majority voting.

### ⚡ Boosting Algorithms
| Algorithm | Key Hyperparameters |
|---|---|
| **AdaBoost** | `n_estimators=100`, `learning_rate=1.0`, Decision Stump base |
| **Gradient Boosting** | `n_estimators=200`, `learning_rate=0.05`, `subsample=0.8`, `max_depth=3` |
| **XGBoost** | `n_estimators=100`, `learning_rate=0.1`, `max_depth=3`, `eval_metric=logloss` |

### 🔷 Support Vector Machines
- **SVC** — Multiclass classification on Iris, with `StandardScaler` preprocessing and kernel comparison.
- **SVR** — Regression on Diabetes dataset with scaled target variable for improved convergence.

---

## 📊 Datasets Used

| Dataset | Source | Task | Samples | Features |
|---------|--------|------|---------|----------|
| **Titanic** | `seaborn.load_dataset` | Binary Classification | 891 | 5 selected |
| **Iris** | `sklearn.datasets` | Multiclass Classification | 150 | 4 |
| **Diabetes** | `sklearn.datasets` | Regression | 442 | 10 |
| **Synthetic Classification** | `make_classification` | Binary Classification | 500 | 20 |
| **Synthetic Regression** | `make_regression` | Regression | 1000 | 10 |

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git https://github.com/saifullah857/Supervised-Learning-Lab.git
cd Supervised-Learning-Lab/supervized02
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter

```bash
jupyter notebook
```

Then open any `.ipynb` file from the browser interface.

---

## 📦 Requirements

```txt
numpy>=1.24
pandas>=2.0
scikit-learn>=1.3
xgboost>=2.0
seaborn>=0.12
matplotlib>=3.7
jupyter>=1.0
```

> Install all at once:
> ```bash
> pip install numpy pandas scikit-learn xgboost seaborn matplotlib jupyter
> ```

---

## 💡 Key Concepts

<details>
<summary><strong>What is Supervised Learning?</strong></summary>

Supervised learning trains a model on **labeled data** — each input has a known output. The model learns the mapping `f(X) → y` and generalizes to unseen data.

- **Classification** — Predict a discrete class label (e.g., survived / not survived).
- **Regression** — Predict a continuous numeric value (e.g., disease progression score).

</details>

<details>
<summary><strong>Bias–Variance Tradeoff</strong></summary>

All notebooks demonstrate this tradeoff:
- A single Decision Tree overfits (high variance).
- Random Forest and Boosting methods reduce variance through aggregation.
- Tuning `max_depth`, `min_samples_leaf`, and `n_estimators` balances bias and variance.

</details>

<details>
<summary><strong>Why Ensemble Methods Work</strong></summary>

Ensemble methods combine multiple weak learners to build a stronger predictor:
- **Bagging** (Random Forest) — Reduces variance by averaging independent learners.
- **Boosting** (AdaBoost, GBM, XGBoost) — Reduces bias by sequentially correcting errors.
- **Voting** — Combines diverse model types for robust predictions.

</details>

---

## 🤝 Contributing

Contributions are welcome! If you'd like to add a new algorithm notebook, improve an existing one, or fix a bug:

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add: your feature"`
4. Push to your branch: `git push origin feature/your-feature`
5. Open a Pull Request

Please ensure notebooks are cleaned of output before submitting (`Kernel → Restart & Clear Output`).

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<div align="center">

Made with ❤️ for Machine Learning learners everywhere

⭐ **Star this repo** if you found it helpful!

</div>