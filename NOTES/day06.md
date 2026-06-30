# Day 6 - Random Forest

## 1. Why Random Forest?

A single Decision Tree can overfit the training data because it may learn very specific rules.

Random Forest solves this problem by combining many Decision Trees and taking the majority vote.

Instead of trusting one tree, it trusts the collective decision of many trees.

---

## 2. What is a Random Forest?

Definition:

Random Forest is an ensemble machine learning algorithm that combines multiple Decision Trees to make better predictions.

"Random" means each tree is trained differently.

"Forest" means a collection of many Decision Trees.

---

## 3. How Does Random Forest Work?

Step 1:
Create multiple Decision Trees.

Step 2:
Each tree is trained using:
- Random samples from the training dataset (Bootstrap Sampling)
- Random subsets of features

Step 3:
Each tree makes its own prediction.

Step 4:
Combine all predictions.

For Classification:
Majority Voting

For Regression:
Average of Predictions

---

## 4. Why Does Random Forest Perform Better?

Since every tree is slightly different, they make different mistakes.

When all trees vote together:

- Wrong predictions from a few trees are outvoted.
- Correct predictions dominate.
- Better generalization.
- Less overfitting.

---

## 5. Decision Tree vs Random Forest

Decision Tree

Advantages:
- Fast
- Easy to understand
- Easy to visualize

Disadvantages:
- Easily overfits
- Sensitive to small changes in data

Random Forest

Advantages:
- Higher accuracy
- More robust
- Less overfitting
- Better generalization

Disadvantages:
- Slower
- Harder to interpret
- Uses more memory

---

## 6. Random Forest Workflow

Dataset

↓

Train-Test Split

↓

Training Data

↓

Random Forest builds many Decision Trees

↓

Each Tree learns independently

↓

Prediction from every Tree

↓

Majority Voting

↓

Final Prediction

---

## 7. RandomForestClassifier()

Example:

model = RandomForestClassifier(
    n_estimators=100,
    random_state=42
)

Parameters:

n_estimators
Number of Decision Trees in the forest.

random_state
Makes random operations reproducible.

---

## 8. What Happens Inside fit()?

model.fit(X_train, y_train)

Internally:

1. Build Tree 1 using random samples and random features.
2. Build Tree 2 using different random samples and features.
3. Repeat until all trees are trained.
4. Store every trained tree.

Important:

Each Decision Tree learns independently.

Trees do NOT learn from each other.

---

## 9. What Happens Inside predict()?

model.predict(X_test)

Process:

A test sample is given to every Decision Tree.

↓

Each tree predicts independently.

↓

All predictions are collected.

↓

Classification:
Majority Vote

Regression:
Average Prediction

↓

Final Prediction

---

## 10. accuracy_score()

accuracy = accuracy_score(y_test, y_pred)

Purpose:

Compares actual labels (y_test) with predicted labels (y_pred).

Used only on the unseen test data.

Never evaluate using the training labels because that measures memorization rather than generalization.

---

## 11. Key Terms

Bootstrap Sampling
Randomly selecting training samples (with replacement) to train each tree.

Majority Voting
The class receiving the highest number of votes becomes the final prediction.

Generalization
The ability of a model to perform well on unseen data.

Ensemble Learning
Combining multiple models to create one stronger model.

---

## 12. Important Interview Points

Q. Why is Random Forest usually better than a Decision Tree?

Answer:
Because it combines predictions from many independently trained Decision Trees, reducing overfitting and improving generalization.

---

Q. What does n_estimators do?

Answer:
It specifies how many Decision Trees are created inside the Random Forest.

---

Q. Why is random_state used?

Answer:
To ensure the same random sampling and random feature selection occur every time, producing reproducible results.

---

## Day 6 Summary

Decision Tree

↓

Can Overfit

↓

Random Forest

↓

Many Independent Decision Trees

↓

Majority Voting

↓

More Accurate

↓

Better Generalization