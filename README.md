# E-commerce Rating Prediction

This repository contains the second part of the analysis of an e-commerce dataset. The goal of this analysis task is to train linear regression models to predict users' ratings towards items. This involves a standard Data Science workflow, including exploring data, building models, making predictions, and evaluating results.

## Dataset

The dataset used in this analysis is a cleaned combined e-commerce sub-dataset, different from the one used in the first part of the analysis. The CSV file is named `cleaned_ecommerce_dataset.csv`.

### Dataset Structure

The dataset includes various features related to user interactions with products, such as ratings, reviews, helpfulness scores, and more.

## Analysis Tasks

The analysis involves the following steps:

1. **Import Cleaned E-commerce Dataset**
   - Load the dataset using the Pandas `read_csv` method.
   - Print the total length of the dataset.

2. **Explore the Dataset**
   - Use `head()` and `info()` methods to get an overview of the data.
   - Calculate correlations between features (helpfulness, gender, category, review) and rating.
   - Convert categorical features into numerical values using `OrdinalEncoder`.
   - Analyze and explain the correlations, identifying the most and least correlated features with the rating.

3. **Split Training and Testing Data**
   - Randomly split the dataset into training and testing sets in two different ratios (90:10 and 60:40).
   - Select the two most correlated features and the two least correlated features for model training.

4. **Train Linear Regression Models**
   - Train four linear regression models under different conditions:
     - Model A: Training/testing data in 90:10 ratio with two most correlated features.
     - Model B: Training/testing data in 90:10 ratio with two least correlated features.
     - Model C: Training/testing data in 60:40 ratio with two most correlated features.
     - Model D: Training/testing data in 60:40 ratio with two least correlated features.

5. **Evaluate Models**
   - Evaluate the performance of the models using Mean Squared Error (MSE) and Root Mean Squared Error (RMSE).
   - Print the results of the four models for both metrics.

6. **Visualize, Compare, and Analyze Results**
   - Visualize the results and provide insightful analysis.
   - Discuss the impacts of feature selection and training/testing data size on model performance.
   - Explain any deviations from expected outcomes.

## How to Run

1. Clone the repository.
2. Ensure you have all necessary dependencies installed (e.g., pandas, scikit-learn, matplotlib).
3. Open the Jupyter notebook and follow the steps outlined to complete the analysis.

## Repository Structure

- `data/` : Contains the dataset used for analysis
- `notebooks/` : Jupyter notebooks with the analysis steps
- `README.md` : This file

## Conclusion

This project demonstrates the process of building and evaluating linear regression models to predict e-commerce ratings based on various features. The analysis highlights the importance of feature selection and the size of training data on model performance.
