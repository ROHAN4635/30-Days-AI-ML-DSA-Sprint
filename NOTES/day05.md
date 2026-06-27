# Day 5 - Cross Validation and Hyperparameter Tuning

## 1. Why Train-Test Split is Not Enough

A single train-test split may give misleading results because the test set could be easier or harder than average.

Example:

Split 1 → Accuracy = 96%

Split 2 → Accuracy = 91%

Different splits can produce different scores.

---

## 2. Cross Validation

Definition:

Cross Validation is a technique used to evaluate a model by training and testing it multiple times on different subsets of the training data.

Purpose:

- More reliable evaluation
- Reduces dependence on one random split
- Better estimate of model performance

---

## 3. K-Fold Cross Validation

The dataset is divided into K equal parts called folds.

Example:

K = 5

Round 1:
Train = Fold 2,3,4,5
Test = Fold 1

Round 2:
Train = Fold 1,3,4,5
Test = Fold 2

This continues until every fold has been used as the validation set exactly once.

Final Accuracy:

Average of all fold accuracies.

---

## 4. Cross Validation vs Train-Test Split

Train-Test Split

- Creates a final unseen test set.
- Used for final evaluation.

Cross Validation

- Performed only on the training data.
- Used to compare and improve models.

Professional Workflow:

Entire Dataset

↓

Train-Test Split

↓

Training Set

↓

Cross Validation

↓

Best Model

↓

Final Test Set

↓

Final Accuracy

---

## 5. cross_val_score()

Purpose:

Evaluates a model using cross validation.

Example:

scores = cross_val_score(model, X, y, cv=5)

Arguments:

model
The machine learning algorithm to evaluate.

X
Feature data.

y
Labels (target values).

cv
Number of folds.

Output:

Returns one score for each fold.

Example:

[0.96, 0.93, 0.97, 0.95, 0.94]

Average:

scores.mean()

---

## 6. Hyperparameters

Definition:

Hyperparameters are settings chosen before training the model.

Examples:

max_depth

random_state

Unlike learned parameters, hyperparameters are decided by the user.

---

## 7. max_depth

Definition:

Controls the maximum depth of a Decision Tree.

Small max_depth

- Simpler tree
- Faster
- May underfit

Large max_depth

- More complex tree
- Learns more details
- May overfit

Choosing the correct depth helps balance learning and generalization.

---

## 8. random_state

Definition:

Controls random decisions made by the algorithm.

Purpose:

- Produces reproducible results.
- Ensures the same model is built every time.

Example:

DecisionTreeClassifier(random_state=42)

---

## 9. Key Learning

Increasing model complexity does not always improve performance.

A good model learns patterns instead of memorizing the training data.