# Skin-Disorder-Prediction
2:-Create a predictive model using machine learning techniques to predict the various classes of skin disease.
Skin Disorder Classification
Overview

This project builds and compares machine-learning models to classify different skin disorders using tabular clinical and histopathological features (not image-based CNNs). The notebook processes the dataset, performs exploratory data analysis (EDA), engineers/combines clinical and histopathological feature sets, and trains multiple supervised models to predict the disorder class.

Dataset

The dataset used in the notebook contains per-sample clinical measurements and histopathological features (e.g., erythema score, scaling, itching severity, microscopic markers). Place the original dataset file (skin_data.csv or the notebook's dataset file) next to the notebook before running.

Features

Clinical features: patient age, symptom scores (erythema, scaling, itching, etc.), and clinical observations.

Histopathological features: microscopic measurements and tissue-level markers recorded for each sample.

The notebook evaluates each feature subset separately and also trains models on the combined feature set; combining clinical + histopathological features produced the most reliable performance.

Approach

Load and clean the dataset; check for missing values and duplicates.

Perform EDA: class balance, feature distributions, boxplots, and correlation analysis to find predictive features.

Preprocess features: scaling/normalization and optional encoding of categorical variables.

Train and compare models: Random Forest, Support Vector Machine (SVM), XGBoost, and a small Neural Network (MLP).

Evaluate models using accuracy, classification reports (precision/recall/F1), and confusion matrices.

Results

Models trained on the combined clinical + histopathological features showed the best performance. Tree-based models (Random Forest and XGBoost) were particularly strong at separating classes; SVM and the MLP also provided competitive results depending on the feature subset and hyperparameters. See the notebook for classification reports and confusion matrices.
