# BRFSS Diabetes Prediction Project

In our **BRFSS Diabetes Prediction** project, we used the [Diabetes Health Indicators Dataset](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset) from Kaggle. We applied dimensionality reduction using **PCA** (both with libraries and from scratch), conducted feature selection using **AIC** and **backward elimination**, and trained an **SVM classifier** with an **RBF kernel**. To address class imbalance, we incorporated **SMOTE** oversampling.

---

## Attempt at a More Ambitious Project

Before finalizing this project, we experimented with a more advanced and ambitious idea: the [Human Protein Atlas Image Classification](https://www.kaggle.com/competitions/human-protein-atlas-image-classification) competition on Kaggle. This task involved predicting **subcellular protein locations** based on **multi-channel microscopy images** (Red, Green, Blue, Yellow).

We built a **custom CNN** for feature extraction and used an **SVM classifier** (One-vs-Rest strategy) for final classification instead of a softmax layer.

- Images were resized to `32×32` and converted to RGB by merging relevant channels.
- After feature extraction, the CNN output was passed to an SVM to predict **multi-label** protein localization.

Despite the extensive effort, we scored a **public leaderboard F1 score of 0.04**, placing around **2000th**, so we decided to prioritize the BRFSS dataset project, where we had better control over **tabular preprocessing and model tuning**.

---

## Takeaway

The Human Protein Atlas project was a valuable experience in handling **high-dimensional biomedical image data** and integrating **CNN-based feature extraction** with traditional machine learning models like **SVM**.

