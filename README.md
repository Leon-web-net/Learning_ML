# ML From Scratch

Classic machine learning algorithms implemented from first principles in Jupyter notebooks, with worked explanations of the maths behind each one. Custom implementations are validated against their scikit-learn equivalents on the same data.

The goal of this repo is understanding, not performance: each notebook derives how the algorithm works before implementing it, rather than just calling a library.

## Contents

### Regression
| Notebook | What's inside |
|---|---|
| `Linear_regression.ipynb` | Linear regression from scratch — gradient descent on MSE, compared against the closed-form/`sklearn` solution |
| `Logistic_regression.ipynb` | Logistic regression from scratch — sigmoid, cross-entropy loss, gradient derivation |
| `NLP_logistic_regression.ipynb` | Logistic regression applied to text classification — feature extraction from raw text |

### Ensemble Methods
| Notebook | What's inside |
|---|---|
| `Decision_Trees.ipynb` | Decision trees — impurity measures, recursive splitting, and where they overfit |
| `Ada_boosting.ipynb` | AdaBoost — sample re-weighting and why weak learners combine into a strong one |
| `Gradient_Boosting_Regression.ipynb` | Gradient boosting for regression — fitting successive learners to residuals |
| `GBM_multiclass.ipynb` | Gradient boosting extended to multiclass classification |

### Preprocessing
| Notebook | What's inside |
|---|---|
| `Feature_encoding.ipynb` | Categorical feature encoding strategies and when each applies |

## Approach

Each notebook follows the same pattern:

1. **The idea** — what problem the algorithm solves and the intuition behind it
2. **The maths** — loss function, update rule or splitting criterion, derived rather than stated
3. **From-scratch implementation** — NumPy/pandas only
4. **Validation** — results compared against the scikit-learn implementation

## Running

```bash
pip install numpy pandas matplotlib scikit-learn jupyter
jupyter notebook
```

---

*Built as a self-study project to understand what ML libraries are doing under the hood.*
