
# Mobile Carrier Plan Prediction: Recommending Smart or Ultra Plans

## Project Description

Mobile carrier Megaline has identified a significant number of subscribers still utilizing their older, legacy service plans. To optimize their service offerings and encourage adoption of modern plans, Megaline aims to develop a machine learning model. This model will analyze historical subscriber behavior data from customers who have already transitioned to the new plans (Smart or Ultra) and recommend the most suitable new plan for legacy users. The goal is to facilitate a smooth transition for existing customers while enhancing business efficiency.

## Analysis Goal

The primary goal of this project is to build a highly accurate classification model that can predict whether a subscriber should be recommended the "Smart" or "Ultra" mobile plan based on their usage patterns and behavior. We aim to achieve the highest possible prediction accuracy, with a specific target threshold of **at least 0.75 (75%)** on the independent test dataset.

This will involve:

* **Data Exploration and Preprocessing:** Understanding the features related to subscriber behavior and preparing the data for machine learning.
* **Model Training:** Investigating and training various classification models suitable for this task.
* **Hyperparameter Tuning:** Optimizing the performance of the chosen models by tuning their hyperparameters.
* **Model Evaluation:** Assessing the final model's accuracy on a separate, unseen test dataset to ensure its generalization capability.

## Technologies Used

* **Python**
* **Pandas:** For efficient data loading, manipulation, and initial data exploration.
* **Scikit-learn:** For machine learning functionalities including:
    * `train_test_split`: For splitting data into training and testing sets.
    * `DecisionTreeClassifier`: A foundational tree-based classification model.
    * `RandomForestClassifier`: An ensemble tree-based classification model, often providing robust performance.
    * `LogisticRegression`: A powerful linear classification model often used as a baseline.
    * `accuracy_score`: The primary metric for model evaluation.
    * `Matplotlib`, `Seaborn`: For data visualization during EDA or result presentation.
* **Jupyter Notebook:** The primary environment for conducting the analysis, experimentation, and presenting findings.

## Dataset

The project utilizes historical subscriber behavior data provided by Megaline, gathered from customers who have already transitioned to the new "Smart" or "Ultra" plans.

* **File Name:** `users_behavior.csv`
* **Content:** This dataset contains various features describing customer usage patterns (e.g., call duration, message count, internet traffic) and the `plan` they ultimately adopted (Smart or Ultra), which serves as the target variable.
* **Original Location (on training platform):** `/datasets/users_behavior.csv`
