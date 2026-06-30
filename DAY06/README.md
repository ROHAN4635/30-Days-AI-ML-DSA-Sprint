# Day 6 - Random Forest

## Topics Covered

- Ensemble Learning
- Random Forest
- Bootstrap Sampling (Concept)
- Majority Voting
- RandomForestClassifier
- n_estimators
- random_state
- fit()
- predict()
- accuracy_score()

---

## Practical Work

- Imported RandomForestClassifier.
- Loaded the Iris dataset.
- Split the data into training and testing sets.
- Built a Random Forest model.
- Understood the role of n_estimators and random_state.
- Trained the model using fit().
- Predicted unseen samples using predict().
- Evaluated model performance using accuracy_score().

---

## Key Learnings

- A Random Forest is a collection of Decision Trees.
- Each tree is trained independently using different random samples and feature subsets.
- Classification is performed using Majority Voting.
- Random Forest reduces overfitting compared to a single Decision Tree.
- More trees generally improve stability and accuracy but increase computation time.
- The model is evaluated only on unseen test data to measure generalization.

---

## Concepts Connected

Decision Tree
→ Overfitting
→ Generalization
→ Random Forest
→ Majority Voting
→ Better Accuracy

---

## Files

notebooks/
- random_forest_intro.ipynb

code/
- (Practice programs if added later)

datasets/
- Iris Dataset

notes/
- day06.md

---

Status

✅ Completed