# Day 4 - Model Evaluation

## 1. Overfitting

Definition:
Model memorizes training data and performs poorly on new data.

Symptoms:

High Training Accuracy
Low Testing Accuracy

Example:

Train = 100%
Test = 62%

---

## 2. Underfitting

Definition:
Model is too simple and fails to learn patterns.

Symptoms:

Low Training Accuracy
Low Testing Accuracy

Example:

Train = 58%
Test = 55%

---

## 3. Good Fit

Definition:
Model learns patterns and generalizes well.

Example:

Train = 95%
Test = 93%

---

## 4. Imbalanced Dataset

Definition:
One class dominates the dataset.

Example:

990 Not Spam
10 Spam

Accuracy can become misleading.

---

## 5. Confusion Matrix

                 Predicted

             Positive Negative

Actual Positive   TP      FN

Actual Negative   FP      TN

---

## 6. True Positive (TP)

Actually Positive
Predicted Positive

---

## 7. True Negative (TN)

Actually Negative
Predicted Negative

---

## 8. False Positive (FP)

Actually Negative
Predicted Positive

Also called:
False Alarm

---

## 9. False Negative (FN)

Actually Positive
Predicted Negative

Missed Detection

---

## 10. Accuracy

Accuracy = (TP + TN) / Total

Measures overall correctness.

---

## 11. Precision

Precision = TP / (TP + FP)

Meaning:

When the model predicts Positive,
how often is it correct?

High Precision:
Few False Positives

---

## 12. Recall

Recall = TP / (TP + FN)

Meaning:

Out of all actual positives,
how many did the model find?

High Recall:
Few False Negatives

---

## 13. Precision vs Recall

Precision:
Prediction Quality

Recall:
Ability to Find Positives

---

## 14. F1 Score

Definition:
Balances Precision and Recall.

Used when both are important.

Higher F1 Score generally indicates better balance.

---

## 15. Metric Selection

Disease Detection:
Prefer High Recall

Fraud Detection:
Prefer High Recall

Injury Prediction:
Prefer High Recall

Spam Detection:
Prefer High Precision