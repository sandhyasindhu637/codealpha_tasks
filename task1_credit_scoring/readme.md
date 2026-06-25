# CodeAlpha Internship — Machine Learning Tasks

machine learning projects completed during the CodeAlpha internship program.

---

## ✅ Task 1 — Credit Scoring Model

**objective:** predict whether a person will default on a loan based on their financial history

**dataset:** Give Me Some Credit — 150,000 real records loaded directly from github

**models used:**
- logistic regression
- decision tree
- random forest

**key features used:**
- credit utilization
- monthly income
- debt ratio
- payment history (late payments)
- age, dependents

**feature engineering done:**
- total late payments (sum of all late payment columns)
- monthly debt amount
- income per dependent
- flag for ever being 90+ days late

**evaluation metrics:** precision, recall, f1-score, roc-auc

**results:**

| model | ROC-AUC |
|---|---|
| logistic regression | ~0.81 |
| decision tree | ~0.85 |
| random forest | ~0.84 |

**best model:** decision tree with ROC-AUC of 0.846

---

## tools used

- python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn
- google colab
