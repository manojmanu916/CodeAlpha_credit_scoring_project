# CodeAlpha_credit_scoring_project

Overview
This repository contains a Jupyter Notebook for building and evaluating machine learning models to predict creditworthiness based on customer data. The models classify customers into binary categories (label: 0 or 1, where 1 likely indicates higher credit risk or approval eligibility). The project uses standard preprocessing techniques and compares three classifiers: Logistic Regression, Decision Tree, and Random Forest.
Key highlights from analysis:

Datasets: Two CSV files provided – a large training set (~8,707 samples) and a small test set (48 samples).
Features: Include demographic and financial attributes like Age, Language, Sex, Marital Status, Has_Credit, Field, Month_of_birth, Day_of_birth, Region, Number_of_credits, Linked_cards, INPS_mln_sum, INPS_yes_no, Score_level, Score_class, Score_point, and Changed_phone_number.
Target: Binary 'label' column (0 for low risk/denied, 1 for high risk/approved – interpret based on context).
Preprocessing: Handles missing values (replaces '-' with NaN, fills with medians or 'Unknown'), label encodes categorical features, and scales numerical features.
Models: Trained on scaled data; evaluated using accuracy, classification report, and confusion matrices.
Results: On the small test set (26 samples with label 0, 22 with label 1), Logistic Regression achieved 100% accuracy. Other models (Decision Tree, Random Forest) may vary but are visualized in the notebook. Note: The test set is small, so results may not generalize; consider cross-validation for robustness.
