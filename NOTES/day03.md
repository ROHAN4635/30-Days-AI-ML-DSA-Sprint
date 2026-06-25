# Day 3 - Supervised Learning and Decision Trees

## 1. Supervised Learning

A type of machine learning where the model learns from Features and Labels.

Examples:
- House Price Prediction
- Student Pass/Fail Prediction
- Disease Detection

---

## 2. Train-Test Split

Purpose:
Evaluate model on unseen data.

Training Data:
Used for learning.

Testing Data:
Used for evaluation.

Example:

80% Training
20% Testing

---

## 3. train_test_split()

X_train, X_test, y_train, y_test = train_test_split(
    X,
    y,
    test_size=0.2,
    random_state=42
)

---

## 4. test_size

Determines percentage of data reserved for testing.

Example:

test_size = 0.2

Means:
20% Testing
80% Training

---

## 5. random_state

Ensures reproducible shuffling.

Example:

random_state = 42

---

## 6. Decision Tree

A supervised learning algorithm that makes decisions using a sequence of questions.

Example:

Study Hours > 5?

Yes → Pass

No → Fail

---

## 7. fit()

model.fit(X_train, y_train)

Purpose:
Train the model.

---

## 8. predict()

model.predict(X_test)

Purpose:
Predict labels for unseen data.

---

## 9. Accuracy

Accuracy = Correct Predictions / Total Predictions

Measures overall correctness.

---

## 10. Decision Tree Visualization

plot_tree()

Purpose:
Display the trained tree graphically.

Important parameters:

feature_names
class_names
filled=True

---

## 11. Reading Tree Nodes

Example:

samples = 54

value = [2,48,4]

class = Versicolor

Meaning:

2 Setosa
48 Versicolor
4 Virginica

Prediction:
Versicolor (majority class)

---

## 12. Types of Nodes

Root Node:
First question.

Internal Node:
Intermediate questions.

Leaf Node:
Final prediction.