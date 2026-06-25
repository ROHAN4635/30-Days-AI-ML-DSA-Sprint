# Week 1 Day 1

## What I learned
- Git workflow (status → add → commit → push)
- Difference between dataset, features and labels
- Loaded the Iris dataset using Scikit-Learn
- Understood that ML learns from labeled examples

## Biggest challenge
- Git authentication and push

## Biggest realization
- I don't need to memorize everything. I need to understand why it works.

## Tomorrow
- Learn Pandas

# Week 1 Day 2 Reflection

1. What is one concept that finally "clicked" today?

2. What concept still feels confusing?

3. If someone asked me "What is NumPy?", could I explain it without Google?

4. What Git command do I now understand the best?

5. One thing I'm proud of today.
# Week 1 - Day 3 Notes
# Topic: Introduction to Machine Learning

---

# 1. What is Machine Learning?

Machine Learning (ML) is a branch of Artificial Intelligence where computers learn patterns from data instead of being explicitly programmed with rules.

Example:
Instead of writing:

if Study Hours > 7:
    Pass

we provide many examples of students' study hours and results, and the computer learns the relationship itself.

Definition:
Machine Learning is the process where a computer learns patterns from data and uses those patterns to make predictions on new, unseen data.

---

# 2. Pattern Learning

Humans learn by observing examples.

Example:

Dog
Dog
Dog
Dog

↓

A new dog appears

↓

Human recognizes it as a dog.

Similarly,

Machine Learning learns patterns from examples rather than fixed rules.

---

# 3. Features

Features are the input variables that help the model make predictions.

Example:

| Study Hours | Sleep Hours | Result |

Features:
- Study Hours
- Sleep Hours

Features are also called Independent Variables or Input Variables.

---

# 4. Label (Target)

The Label is the output that we want the model to predict.

Example:

| Study Hours | Sleep Hours | Result |

Label:
Result

The Label is also called:
- Target
- Output Variable
- Dependent Variable

Easy way to identify a label:

Ask yourself,

"What am I trying to predict?"

The answer is the Label.

Everything else becomes Features.

---

# 5. Supervised Learning

Supervised Learning is a type of Machine Learning where the model learns from labeled data.

The dataset contains:

Features + Correct Answers (Labels)

The model learns the relationship between them.

Example:

| Hours | Result |

2 → Fail

8 → Pass

10 → Pass

The model learns the pattern and predicts the result for new students.

Definition:

Supervised Learning is a machine learning technique where the model is trained using labeled data to predict outputs for unseen data.

Examples:
- Spam Detection
- House Price Prediction
- Student Result Prediction
- Football Match Prediction

---

# 6. Training Data

Training Data is the portion of the dataset used to teach the model.

The model studies the patterns from this data.

Purpose:
Learning

---

# 7. Testing Data

Testing Data is the unseen portion of the dataset used to evaluate the model.

The model has never seen this data before.

Purpose:
Evaluation

---

# 8. Why Do We Split Data?

If the model learns using all the data, we cannot know whether it truly learned patterns or simply memorized them.

Therefore,

Dataset

↓

Training Set (usually 80%)

↓

Testing Set (usually 20%)

This helps us measure how well the model performs on new data.

---

# 9. Accuracy

Accuracy tells us how many predictions the model made correctly.

Formula:

Accuracy = Correct Predictions / Total Predictions

Example:

Correct Predictions = 190

Total Predictions = 200

Accuracy = 190 / 200 = 95%

Higher Accuracy generally indicates better performance.

Note:
Accuracy is the first evaluation metric we learn.
More advanced metrics like Precision, Recall and F1 Score will be studied later.

---

# 10. Complete Machine Learning Pipeline

Real World Data

↓

Dataset

↓

Pandas (Understand the data)

↓

NumPy (Efficient numerical arrays)

↓

Train-Test Split

↓

Choose Model

↓

Train Model

↓

Prediction

↓

Evaluate Accuracy

---

# Interview Points

Q. What is Machine Learning?

Machine Learning is the process where a computer learns patterns from data and uses them to make predictions on unseen data.

Q. What are Features?

Features are the input variables used by the model to make predictions.

Q. What is a Label?

The Label is the target output that the model tries to predict.

Q. What is Supervised Learning?

It is a type of machine learning where the model learns from labeled data containing both features and correct outputs.

Q. Why do we split data?

To evaluate whether the model can generalize to unseen data instead of memorizing the training data.

Q. What is Training Data?

Data used to teach the model.

Q. What is Testing Data?

Data used to evaluate the model on unseen examples.

Q. What is Accuracy?

Accuracy is the percentage of correct predictions made by the model.

Formula:


## Day 3

### Topics Learned
- Supervised Machine Learning
- Features and Labels
- Train-Test Split
- Decision Tree Classifier
- Model Training
- Prediction
- Accuracy
- Decision Tree Visualization

### Challenges Faced
- Understood why variable order matters during tuple unpacking.
- Learned why restarting the Jupyter kernel removes variables.
- Resolved matplotlib installation issue.
- Learned how Decision Trees make predictions.

### Biggest Learning
A Decision Tree does not memorize answers. It learns a sequence of decision rules from the training data and predicts the majority class at the leaf node.

### Confidence
⭐⭐⭐⭐☆ (4/5)

### Next Goal
Learn Overfitting, Underfitting and Model Evaluation Metrics.

## Day 4

### Topics Learned
- Overfitting
- Underfitting
- Confusion Matrix
- Accuracy
- Precision
- Recall
- F1 Score

### Biggest Learning
A model with higher accuracy is not always better. The choice of evaluation metric depends on the real-world problem and the cost of different types of mistakes.

### Challenges Faced
- Understanding why accuracy can be misleading.
- Differentiating between Precision and Recall.

### Confidence
⭐⭐⭐⭐☆ (4/5)

### Next Goal
Learn how to improve models and understand cross-validation.