# Iris Flower Classification

## Project Overview

This project uses machine learning to classify Iris flowers into three species: Setosa, Versicolor, and Virginica. The classification is based on four flower measurements: sepal length, sepal width, petal length, and petal width.

The project demonstrates the process of loading and exploring a dataset, preparing data for machine learning, training classification models, and evaluating their performance.

## Objective

To build and compare two machine learning classification models and identify a suitable model for predicting Iris flower species based on their measurements.

## Dataset

The project uses the built-in Iris dataset provided by Scikit-learn.

- **Total observations:** 150
- **Measurement features:** 4
- **Target classes:** 3
- **Observations per species:** 50
- **Missing values:** None

The four measurement features are sepal length, sepal width, petal length, and petal width.

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Project Workflow

1. Introduce the project and load the Iris dataset.
2. Perform exploratory data analysis (EDA) and discuss feature selection.
3. Prepare the data and split it into training and testing sets.
4. Train Logistic Regression and K-Nearest Neighbors (KNN) classification models.
5. Evaluate both models using accuracy, confusion matrices, precision, recall, and F1-scores.
6. Compare model performance, identify the preferred model based on the results, and summarise the findings.

## Exploratory Data Analysis

Exploratory data analysis included examining the dataset's structure, data types, missing values, descriptive statistics, and species distribution.

Pairplots and box plots were used to visualise relationships between measurements and differences between species. Petal length and petal width appeared particularly useful for distinguishing the species.

## Machine Learning Models

Two classification algorithms were trained:

1. **Logistic Regression**
2. **K-Nearest Neighbors (KNN)** with 5 neighbors

The dataset was split into 80% training data and 20% testing data. Stratified sampling was used to preserve the species distribution. StandardScaler was applied within pipelines to scale the features without fitting the scaler on the test data.

## Model Evaluation

Both models were evaluated using accuracy, confusion matrices, precision, recall, and F1-score.

| Metric | Logistic Regression | KNN |
|---|---:|---:|
| Accuracy | 93.33% | 93.33% |
| Macro Precision | 0.9333 | 0.9444 |
| Macro Recall | 0.9333 | 0.9333 |
| Macro F1-Score | 0.9333 | 0.9327 |

## Conclusion

Both models achieved 93.33% accuracy on the test dataset, correctly classifying 28 of the 30 observations.

Logistic Regression was selected as the preferred model for this project because it demonstrated more balanced recall across the three species. KNN achieved slightly higher macro precision but misclassified two Virginica flowers as Versicolor.

The results indicate that both algorithms performed well on this dataset. Since the evaluation used a single train-test split, cross-validation could be used in future work to assess how consistently the models generalise to unseen data.

## Project Files

- `Iris_Flower_Classification.ipynb` — Jupyter Notebook containing the code, visualisations, evaluation results, and conclusions.
- `screenshots/` — Screenshots of relevant project outputs and visualisations.

## Author

Oasis Infobyte Data Science Internship Project
