---
title: "Mushroom Classifier: Predicting Edibility from Morphological Features"
date: 2025-03-27
summary: "A machine learning model that classifies mushrooms as edible or poisonous based on their physical characteristics."
---

**Mushroom Classifier** is a supervised learning project. The goal was to create a robust classifier that could accurately predict whether a mushroom is **edible or poisonous**, based on features such as color, odor, gill shape, and cap surface. The final model used a **Support Vector Classifier (SVC)**, carefully tuned to prioritize safety by minimizing **false negatives**—cases where a poisonous mushroom is incorrectly predicted as edible. While false positives may lead to discarding safe mushrooms, they pose no risk to human health. In contrast, the model was designed to **avoid false negatives** as much as possible, which could lead to real danger if deployed.

#### 🧪 Project Highlights
- **Data preprocessing**: Cleaned and encoded categorical features from the UCI Mushroom dataset.
- **Model comparison**: Evaluated several models including logistic regression, decision trees, and random forests using **cross-validation** and **grid search**.
- **Performance metrics**: Focused on **recall** (to minimize the risk of misclassifying poisonous mushrooms) while maintaining good precision and accuracy.
- **Model interpretation**: Used feature importance analysis and decision plots to explain predictions.

#### 🚀 Results
- **Accuracy:** 0.99 on unseen test data  
- **F2 Score (β=2):** 0.99  
- **Correct Predictions:** 12,174 out of 12,214  
- **Errors:**
  - 17 false negatives (poisonous predicted as edible)
  - 23 false positives (edible predicted as poisonous)

[🔗 View on GitHub](https://github.com/UBC-MDS/mushroom_classifier)
